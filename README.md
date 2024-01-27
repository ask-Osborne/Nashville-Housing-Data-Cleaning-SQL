![nashville](https://github.com/ask-Osborne/Nashville-Housing-Data-Cleaning-SQL/assets/154265439/7ec4d6c6-31ce-4240-8999-687d6c6d5236)
# Nashville Housing Data Analysis and Cleaning

## Overview

This project focuses on the analysis and cleaning of Nashville Housing data. The SQL queries provided aim to standardize date formats, populate missing property addresses, break down addresses into individual columns, split owner addresses, change 'Y' and 'N' to 'Yes' and 'No' in the "Sold as Vacant" field, remove duplicate records, and delete unused columns.

## SQL Queries

### Step 1: Standardize Date Format

The SaleDate column is standardized to the date format.

### Step 2: Populate Missing Property Address Data

Missing PropertyAddress values are populated by leveraging data from other rows with the same ParcelID.

### Step 3: Break Out Address into Individual Columns

The PropertyAddress column is split into PropertySplitAddress and PropertySplitCity.

### Step 4: Split Owner Address into Individual Columns

The OwnerAddress column is split into OwnerSplitAddress, OwnerSplitCity, and OwnerSplitState.

### Step 5: Change Y and N to Yes and No

The "Sold as Vacant" field is updated to replace 'Y' with 'Yes' and 'N' with 'No'.

### Step 6: Remove Duplicate Records

Duplicate records are removed, keeping only one unique record for each combination of ParcelID, PropertyAddress, SalePrice, SaleDate, and LegalReference.

### Step 7: Delete Unused Columns

Unused columns (OwnerAddress, TaxDistrict, PropertyAddress, SaleDate) are dropped from the table.

## Usage

Execute the provided SQL queries in sequence to perform the analysis and cleaning steps. Adjust database and table names as needed.

Feel free to explore and adapt the queries based on specific requirements.

## Note

Make sure to backup your data before executing any modifications, especially if the SQL queries are run on a production database.



