# Project Ephesus
- [Introduction](#introduction)
- [Highlights](#highlights)
- [Usage](#Usage)
- [Requirements](#Requirements)
- [Contributing](#Contributing)
- [License](#License)

## Introduction
The workflow aims to establish a user-level datamart that is highly flexible for seamless integration with CRM data. The system includes built-in fields representing essential user information, such as geographic data, traffic sources, purchase behavior, and engagement behavior. The entire segmentation stage can be orchestrated efficiently using Google Colab.

Easily create a single holistic view of all customers by joining GA4 data with CRM data.
Flexible for various (generic or custom)  segmentation use cases and experimentation with modeling (clustering methods, rule-based segmentation, ml based segments, dashboarding, automated activation etc.).
Can be easily integrated with Customer Match using Ads Api or Google Ads Data Manager.


## Highlights

1. **Holistic Customer View**
   
Creates a unified view of all customers by seamlessly joining GA4 data with CRM data. The output table data dictionary can be found inside google colab notebook.
  - Flexible Segmentation
  - Clustering methods
  - Rule-based segmentation
  - ML-based segments
  - Dashboarding

2. **Measurement Use Case Flexibility**
  - Enables the creation of datamarts for different time windows, catering to diverse measurement use cases.

3. **Automation of Activation (Integration with Customer match using ads api)**
  - Easily integrates with Customer Match through Ads API, providing enhanced advertising capabilities. (Recommended to test with Google Ads Data Manager)

## Usage
Here is the link to the google colab notebook.
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.sandbox.google.com/drive/1KTo9Vlz49kJ6FHPaOFuZNZ9wv0Z3-nzl?pli=1#scrollTo=2aOzphABtGV0)


Follow the brief instructions in the colab notebook.

## Requirements

To deploy the workflow successfully:

**GA4 Setup:**
   - Validate correct flow of Purchase/E-Commerce events in GA4.
   - Define and transfer User ID to the website data layer using GTM.
   - Identify and introduce product-related fields using GTM.
   - Set up the BigQuery GA4 link, enable Google Signals, and authorize users in GA4.
   - Optionally configure data retention and implement E-Commerce events.
**BigQuery Configuration:**
   - Create a project, configure billing settings, and grant access to project members.
**CRM Data Management:**
   - Maintain and update user-level data in CRM, including User ID and corresponding hashed-email, user_id.
   - Optionally include phone and address information.
**Customer Match Automation:**
   - optional: Obtain a developer's API token for uploading customer lists to Google Ads using API.
   - optional: Test with Google Ads Data Manager

## Contributing
We welcome contributions from the open-source community!

[Details](CONTRIBUTING.md)

## License
This project is licensed under the [Apache License](LICENSE).

--
*This is not an officially supported Google product.*


