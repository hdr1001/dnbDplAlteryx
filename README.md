# dnbDplAlteryx
D&amp;B Direct+ endpoints implemented in Alteryx workflows

## Required
1. for authentication workflow ➡️ environment variables: DnbDplKey & DnbDplSecret for API credentials
2. for other workflows ➡️ environment variables: DnbDplToken

I have not found a way to get around closing and re-starting Alteryx Designer after changing environment variables

## Example 
![image](https://github.com/user-attachments/assets/2f57a92b-3f3e-4e2d-a2fc-25ded7d1e1c6)

Please note: As mentioned in the license distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.

## Implemented transactions

- [authentication](https://directplus.documentation.dnb.com/html/pages/Authentication.html) Please note: implemented v2
- check_auth, a reference data request to check the validity of the authorization token
- [entitlements](https://directplus.documentation.dnb.com/openAPI.html?apiID=entitlements) Check the API credentials entitlement
- [reference_cats](https://directplus.documentation.dnb.com/openAPI.html?apiID=refDataCategories) List the available reference categories
- [reference_cat](https://directplus.documentation.dnb.com/openAPI.html?apiID=refDataCodes) List the codes in a reference category
- [id_resolution](https://directplus.documentation.dnb.com/openAPI.html?apiID=IDRCleanseMatch) IDentity Resolution (aka cleanse match)
- [data_blocks](https://directplus.documentation.dnb.com/DataBlocks.html) Data block enrichment request
- [full_fam_tree](https://directplus.documentation.dnb.com/openAPI.html?apiID=familyTreeFull) Full family tree enrichment request
