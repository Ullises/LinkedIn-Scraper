# Enterprise Web Scraper for LinkedIn

## Introduction to LinkedIn ![LinkedIn Logo](https://cdn-icons-png.flaticon.com/512/174/174857.png)

LinkedIn is a premier professional networking platform, designed to connect professionals and businesses worldwide. Owned by Microsoft, it serves as a hub for individuals seeking career advancements and businesses aiming to foster professional relationships.

## Key Features
- **Profile Optimization:** Create a comprehensive professional profile showcasing your skills, experiences, and achievements, allowing you to stand out in the competitive job market.
- **Connect with Your Network:** Start by connecting with colleagues, classmates, mentors, and other professionals in your industry.
- **Join Groups and Follow Influencers:** Engage with industry-specific groups and follow influential thought leaders to stay updated on relevant discussions and trends.
- **Content Sharing and Insights:** Share industry insights, thought leadership articles, and engage with a global professional community through posts, articles, and comments.
- **Company Pages:** Gain insights into prospective employers or clients by exploring their company pages, which highlight their mission, culture, job openings, and more.
- **Messaging and Communication:** Foster meaningful connections through private messaging, allowing for direct communication with fellow professionals.
  
## Enterprise Web Scraper for LinkedIn ![Microsoft Logo](https://www.pngmart.com/files/4/Microsoft-Logo-PNG-Transparent-Image.png)

Web scraping is a powerful tool for data-driven companies aiming to extract valuable insights from various online sources. Our Enterprise Web Scraper for LinkedIn is designed to:

- Extract and analyze data for market research.
- Monitor and compare pricing strategies of competitors.
- Gather insights from forums and social platforms.

However, it's essential to use web scraping responsibly, ensuring compliance with terms of service and copyright laws.

Our tool specifically targets LinkedIn, enabling businesses to delve deeper into their professional networks, visualize connections, and derive actionable insights.

## Installation and Usage

### Setting Up

1. **Dependencies Installation**:
   Begin by executing the Python script to install the necessary libraries:

   Execute chromedriver file
pip3 install -r requirements.txt


2. **Initiate Extraction**:

```python
python3 extraction.py
```


3. **Login Credentials**:
Provide your LinkedIn username and password. Rest assured, your password remains confidential and won't be displayed.

4. **Select Contacts**:
Post login, the scraper will navigate to your contacts. Specify the number of contacts you wish to scrape. Note: The number of contacts affects the scraping duration.

5. **Data Extraction**:
The tool will display the selected contacts and initiate the scraping process. Upon completion, you'll receive a status update for each contact.

6. **Visualization**:
Once the extraction is complete, you can choose to render the data into a visual graph. This will generate an `.html` file, which can be viewed in any web browser.

## Technical Overview

### Data Extraction

Our tool employs various Python functions to navigate and extract data from LinkedIn:

- **Login**: Automates the login process.
- **Navigation**: Directs the scraper to the contacts page and expands the list.
- **Contact Extraction**: Retrieves the list of your contacts.
- **Friend's Contacts**: Gathers a list of contacts from your connections.
- **Profile Visit**: Visits each profile and extracts data.
- **Data Selection**: Allows users to specify the number of contacts for scraping.

### Network Creation & Visualization

Post data extraction, our tool creates a network graph using the NetworkX library:

- **Node Addition**: Maps the network and creates nodes.
- **Edge Creation**: Generates links between you, your contacts, and their connections.

Finally, the network is saved as a `linkedin_graf.gexf` file. For visualization, we utilize the Pyvis library to transform the NetworkX graph into an interactive visualization, saved as `my_graf.html`.

## Conclusion

Our Enterprise Web Scraper for LinkedIn is a robust tool designed for businesses aiming to harness the power of their professional network. By providing a deeper understanding of connections and facilitating data-driven decisions, this tool is an invaluable asset for modern enterprises.

   
