

# ETL AMI - Data Description Document:

## Required & Commonly Used Fields
Cite [Department of Transportation Documentation](https://www.transportation.gov/sites/dot.gov/files/docs/mission/gis/national-address-database/308816/nad-schema-v2.pdf)

## id:
### description: 
- Original primary key in Data Pipeline SQL table
### example: `1`

## address_objectid:
## description:
- Object ID from National Address Database (NAD)
### example: `13651367`

## fips2010:
### description:
- THIS WILL CHANGE!
- Counties & county subdivisions from HUD
- There exists a *more* authoritative version: Census Based Statistical Area
- AKA: the key back into HUD's 80% Income Limit data 
### example: `1800199999`

## tract_id:
### description:
- Census Tract 
### example: `18001030500`

## does_income_qualify:
### description:
- Is the tract a "low income area" qualified by Renter AMI
- "Is the tract Renter AMI < HUD income limit?"
### example: `True`

## hud_income_limit:
### description: 
- 80% AMI for the HUD area for a family of 1
### example: `37450`

## tract_median_renter_income:
### description:
- AMI for Renters in tract
### example: `30179.0`

## state:
### description:
- USPS state code 
### example: `IN`

## county:
### description:
- Name of county the address resides in
- In non-Native areas there is 1:1 tract and address 
### example: `Adams`

## inc_muni:
### description:
- TBD 
- Name of the incorporated municipality or other general - purpose local governmental unit where the address is located
### example: 

## uninc_comm:
### description:
- TBD 
- Name of an "unincorporated community", either within an incorporated municipality or in an unincorporated portion of a county, or both where the address is located.
### example: 

## nbrhd_comm:
### description: 
- Name of an unincorporated neighborhood, subdivision or area, either within an incorporated municipality or in an unincorporated portion of a county or both, where the address is located.
### example: 

## post_comm:
### description: 
- A city name for the ZIP code of an address, as given in the USPS City State file
### example: `BLUFFTON`

## zip_code:
### description: 
For standard street mail delivery (with a corresponding geographic delivery area), the system of 5-digit codes that identifies the individual USPS Post Office associated with an address.
### example: `46733`

## plus_4:
### description:
- The ZIP plus 4 code (without the dash)
### example: `1234`

## stn_premod:
### description: 
- For Bulk Delivery (e.g., government mailroom) zip codes with no corresponding geographical area, the system of 5-digit codes that identifies the individual delivery location associated with an address
### example: 

## stn_predir:
### description:
- Word preceding the Street Name element that indicates the direction taken by the street from an arbitrary starting point or line, or the sector where it is located
### example: `South`

## stn_pretyp:
### description:
- Word or phrase that precedes the Street Name element and identifies a type of thoroughfare in a complete street name
### example: 

## stn_presep:
### description: 
- Preposition or prepositional phrase between the Street Name Pre-Type and the Street Name
### example: 

## streetname:
### description: 
- The element of the complete street name that identifies the particular street (as opposed to any street types, directionals, and modifiers). At this time, if the point represents a milepost or landmark, this field will not be required
### example: `700`

## stn_postyp:
### description: 
- Word or phrase that follows the Street Name element and identifies a type of thoroughfare in a complete street name
### example: 

## stn_posdir:
### description: 
- A word following the Street Name element that indicates the direction taken by the street from an arbitrary starting point or line, or the sector where it is located.
### example: `West`

## stn_posmod:
### description: 
- A word or phrase that follows and modifies the Street Name element, but is separated from it by a Street Name Post Type, a Street Name Post Directional, or both
### example: 

## addnum_pre:
### description: 
- An extension of the Address Number that precedes it and further identifies a location along a thoroughfare or within a defined area
### example: 

## add_number:
### description: 
- The whole number identifier of a location along a thoroughfare or within a defined community. At this time, if the point represents a milepost or landmark, this field will not be required
### example: `145`

## addnum_suf:
### description: 
- An extension of the Address Number that follows it and further identifies a location along a thoroughfare or within a defined area.
### example: 

## unit:
### description: 
- A group or suite of rooms within a building that are under common ownership or tenancy, typically having a common primary entrance.
### example: 

## longitude:
### description: 
- Address Longitude, derived based on point placement
### example: `-85.0680406229999`

## latitude:
### description: 
- Address Longitude, derived based on point placement
### example: `40.740386394`
