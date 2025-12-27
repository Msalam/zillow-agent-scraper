# 🚀 Zillow Agent Data Scraper (High-Resilience)

An automated data extraction solution designed to scrape detailed real estate agent profiles from Zillow. This project leverages ScrapingBee for JavaScript rendering and proxy rotation to ensure high delivery rates and bypass sophisticated anti-bot measures.

---

## 🎯 Business Value (Client Perspective)

This tool is engineered to provide high-quality lead generation data with zero manual effort.

- **Accurate Data Extraction**: Delivers clean, structured CSV files containing agent names, contact details, sales history, and experience levels.  
- **Anti-Block Technology**: Built-in integration with premium proxies and residential IPs to ensure the scraper never gets blocked or throttled by target websites.  
- **High Efficiency**: Uses multi-threading to fetch data rapidly while maintaining a "human-like" request pattern to protect the account's reputation.  
- **Set-and-Forget Automation**: Once configured, the script handles retries, JS rendering, and data storage without requiring technical intervention.  

---

## 🛠️ Technical Architecture (Developer Perspective)

Built with scalability and resilience in mind, the script addresses common scraping challenges:

- **Dynamic Content Handling**: Utilizes ScrapingBee API to render heavy JavaScript content, ensuring data hidden behind React/Next.js components is fully captured.  
- **Concurrency**: Implements `ThreadPoolExecutor` for parallel processing, significantly increasing throughput compared to sequential scraping.  
- **Resilience Framework**:
  - **Retry Logic**: Automatically retries failed requests (up to 3 times) with randomized exponential backoff.  
  - **Error Handling**: Captures and logs failed URLs separately to ensure no data loss during network fluctuations.  
  - **API Optimization**: Configured to use `premium_proxy` and `country_code` parameters to maximize the success rate per API credit.  

---

## 📊 Data Points Collected

The scraper extracts the following fields into a structured CSV:

- Agent Title/Name  
- Email Address  
- Phone Number  
- Fax Number  
- Office Address  
- Sales in the last 12 months  
- Total Lifetime Sales  
- Price Range of Properties  
- Average Property Price  
- Years of Experience  

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8+  
- ScrapingBee API Key  
- Google Colab (Optional, configured for Drive storage)  

### Installation

Clone the repository:

```bash
