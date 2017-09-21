# GTS APIs
## What is GTS?
Global Trade Solution(GTS) enables users to calculate import duty and taxes in a few quick steps, when you are importing goods into the USA, EU, Russia, Canada and many more countries. Along with Duty & Taxes, GTS also returns if there is any applicable restriction.

# API Details
```
API URL:                http://www.dutycalculator.com/api2.1/sandbox/
API key for Sandbox:    2bac6dba1354599a
Reference document:     https://docs.google.com/document/d/1_C5XqlAOlw_jv62idHev5Dpu6z6clxFk9l4q_M_OAvs/pub 
```
Note: This is a sandbox account. All the API validations will be done however the response for any request will be static.</b>

For Instance, 
```
REQUEST: http://www.dutycalculator.com/api2.1/sReferandbox/2bac6dba1354599a/get-hscode?from=usa&to=ind&desc[0]=waterBottle&detailed_result=1

RESPONSE:

<classifications country-to-code3="IND">
	<classification quality-score="high">
		<hs-code>8517.12.90</hs-code>
			<short-commodity-description>
				<![CDATA[
				Telephone | mobile phone (Phones, Pagers & PDAs: Electronics & Video Games)
				]]>
			</short-commodity-description>
		<duty-category-description>
		<category id="L1-145">Electronics & Video Games</category>
		<subcategory id="L2-135">Phones, Pagers & PDAs</subcategory>
		<item id="844">Telephone | mobile phone</item>
		</duty-category-description>
		<duty>
			<![CDATA[ 0% ]]>
		</duty>
		<sales-tax name="GST">
			<![CDATA[ 12% ]]>
		</sales-tax>
		<additional-import-taxes>
			<tax name="Landing charges">
				<![CDATA[ 1% CIF ]]>
			</tax>
			<tax name="CESS">
				<![CDATA[
				0% (Duty + Landing charges + CEX (Education &amp; Higher Education CESS) + Countervailing duty)
				]]>
			</tax>
		</additional-import-taxes>
		<import-restrictions>
			<![CDATA[
			Importation of articles without an International Mobile Equipment Identity (IMEI), Electronic Serial Number (ESN), Mobile Equipment Identifier (MEID) is prohibited, controlled by the Department of Commerce and the Indian Customs Office. Please contact agency for more information. [High Probability]
			]]>
		</import-restrictions>
		<export-restrictions>
			<![CDATA[
			This product has dual-use and therefore requires an Export Control Classification Number (ECCN).
			]]>
		</export-restrictions>
		<carrier-restrictions>
			<![CDATA[
			Restrictions will apply for shipping this product with courier or postal companies. Please note that shipping prohibitions, restrictions (articles with SIM cards/without) and special packaging requirements may apply to these articles. Please contact your courier for more information.
			]]>
		</carrier-restrictions>
	</classification>
</classifications>

```
