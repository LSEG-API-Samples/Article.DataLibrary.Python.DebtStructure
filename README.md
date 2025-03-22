# Debt Structure Analysis on an Organizational Level

Many times when one is looking to analyze the Debt Structure of an issuer within the desktop using LSEG Workspace, the first thought is to look at the Debt Structure page. This is an excellent resource to analyze all bonds that meet specific requirements be it Maturity, Capital Tier, Coupon Class amongst many other categories. Not only does this information give us insight into the debt obligations of said organization, but it also sheds light into the burdens of future coupon payments, the distribution of risk and the implications in new areas such as Green Bonds.

With this article we would like to bring this kind of analysis to life through the use of the LSEG Data Library for Python. We will go through some simple steps to search for all the bonds for a given issuer, look at some of the most relevant fields for the active bonds, and we will standardize the currency so we can look at the total value of the obligations in a single currency. This is done with the intent of explaining how to use the Search API functionality, how we can organize the properties/fields we're interested in, how to implement FX conversion from the currency of issue to a chosen FX snapshot and then ultimately look at the overall obligations by subsidiary but also as a whole.

Refer to the [Debt Structure Article](https://developers.lseg.com/en/article-catalog/article/debt-structure-analysis-on-an-organizational-level) defined within the LSEG Developer Community for more details.

***Note:** To [ask questions](https://community.developers.refinitiv.com/index.html) and benefit from the learning material, I recommend you to register on the [LSEG Developer Community](https://developers.lseg.com)*

## <a name="prerequisites"></a>Prerequisites

[Development Environment](https://developers.lseg.com/en/api-catalog/lseg-data-platform/lseg-data-library-for-python/quick-start#getting-started-with-python)

- Notebook can be directly loaded into the LSEG Workspace CodeBook development environment
- Packages: [data library](https://pypi.org/project/lseg-data/) [pandas](https://pypi.org/project/pandas/) numpy matplotlib
- LSEG Data Library for Python installation:  '**pip install lseg-data**' (if running outside of CodeBook)

## <a name="setup"></a>Setup

The package includes a single Jupyter Notebooks demonstrating features of the service.  Depending where you plan to access the content from, you will need provide the proper credentials:
* **Desktop Access**
  
  The notebook has been set up and tested to access data within the desktop when running **LSEG Workspace**.
  
* **Platform Access**
  
  If you have an RDP license, refer to the [Session Example](https://github.com/LSEG-API-Samples/Example.DataLibrary.Python/blob/lseg-data-examples/Examples/4-Session/EX-4.01.01-Sessions.ipynb) for details.

### <a id="authors"></a>Authors

* **Nick Zincone**
* **Simone Da Costa**
