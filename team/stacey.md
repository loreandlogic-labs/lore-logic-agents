# Stacey

## Goal for this program

Get good enough at building agents to ship reliable ones for real work at Lore and Logic.

## Flagship project (under consideration)

**Land report agent**: reads a land title along with other public inputs, such as topography, and produces a report that helps a buyer make an informed decision about a property.

### Inputs

- **Land title**: owners, charges, liens, easements and covenants.
- **Topography**: slope, elevation and drainage.
- **Zoning and bylaws**: permitted uses, setbacks and development restrictions.
- **Flood and hazard maps**: floodplain, wildfire, slope stability and contamination.
- **Wetland and environmental rules**: wetland policy and similar acts that limit what can be built or disturbed.
- **Servicing and access**: road access, water, septic or sewer, and power.
- **Comparable sales**: recent nearby sales and assessed value.

### Components

- **Title extraction agent**: pulls the key facts out of the land title.
- **Research agents**: gather and summarize each of the other inputs.
- **Red-flag agent**: looks across all the inputs for issues a buyer should know about.
- **Report agent**: writes the final report, with every claim citing its source document.

### Plan

- **First:** get title extraction working well on a handful of sample titles.
- **Then:** add the other inputs one at a time.
- **After that:** produce full reports and compare them with my own reviews.

### Evals

- **Extraction accuracy**: are owners, charges, liens, easements and covenants pulled from the title correctly?
- **Red-flag recall**: does the report catch every issue a professional would flag?
- **Citation accuracy**: does every claim trace back to a source document?
- **Expert agreement**: how closely do the report's conclusions match my own hand-written reviews?
