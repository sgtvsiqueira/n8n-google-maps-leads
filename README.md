# n8n Google Maps Lead Generator

**Brief description**: n8n workflow for automated lead generation using Google Maps Places API

## Features
- Automated business data extraction from Google Maps Places API
- Google Sheets integration for data storage and management  
- Configurable ZIP code and business category filtering
- Rate limiting with exponential backoff error handling
- Duplicate detection and data deduplication
- Scheduled execution with manual trigger options

## Installation
1. Import workflow JSON into n8n instance
2. Install required community nodes (none required)
3. Create API credentials:
   - Google OAuth2 API key for Places API
   - Google Service Account for Sheets access
4. Configure in respective developer portals:
   - Enable Google Places API (New) 
   - Enable Google Sheets API
   - Set permissions and scopes for service account
   - Configure webhook URLs (not required for this workflow)

## Setup Requirements
- n8n instance (self-hosted or cloud)
- Google Cloud Platform account and API access
- Required credentials configured
- Google Sheets document with proper structure

## Configuration
1. Update Settings node with your Google Sheets URL
2. Configure ZIP codes sheet with status column
3. Set up business categories in Google Maps Categories sheet
4. Ensure proper column mapping in Google Sheets nodes

## Version Info
- Latest: v1.0.0
- Recent additions:
  - Exponential backoff retry logic
  - Google Sheets status tracking
  - Configurable business categories

## Compatibility
- Fair-code licensed
- Requires n8n workflow platform
