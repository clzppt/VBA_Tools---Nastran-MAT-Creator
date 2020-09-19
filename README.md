# VBA_Tools---Nastran-MAT-Creator

Excel VBA tool to create a material database which can be used to write out .bdf files (for use with NASTRAN).

The intended use for this spreadsheet is for multiple users in a working group to add appropriate FEM material properties to a "database" which all group members can then use to have access to consistent material property values.  As the database grows, the users can then select only the materials they need for their new model and quickly create the MAT cards needed.

- Currently supports MAT1, MAT2, and MAT8 NASTRAN material definitions with 1, 2, or 3 input rows
- Writes a unique .bdf file for each card type (e.g. if you need all three material types, run all three macros)
- Output .bdf includes hypermesh 2019 style comments to populate material descriptions, and material
  color (increments color # for each material) when imported to the a .HM model
