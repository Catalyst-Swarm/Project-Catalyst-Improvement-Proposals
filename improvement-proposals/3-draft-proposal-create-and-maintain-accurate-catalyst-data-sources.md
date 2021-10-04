# \#3 - Draft Proposal - Provide accurate Catalyst data sources

### **Problem‌**

The community doesn't have accurate access to Catalyst data that are needed to create improved processes and tools for the ecosystem

### **Solution‌**

Create open source data repositories for the Catalyst data sources that the community can use for creating better processes and tools

### Vote

**TODO** - Add voting if required.

## **Research and analysis**

#### **Overview**

To improve and replace existing parts of the Catalyst ecosystem the community needs access to accurate data sources for the existing tools and processes.

**Why is accurate open data access important?** 

* Anyone in the community should be able to use Catalyst data to create their own ideas for solutions
* The community can create solutions that mirror existing tool and process data which means offering low risk and high value alternatives that can be more easily used by the community. This approach allows the community to gradually start using alternative solutions before anything gets fully endorsed as a preferred solution
* If data is open source and accurate it will be easier to promote this to the community and encourage more solutions to be developed
* Data can be combined and turned into a Catalyst data API based off of accurate raw data

**Why is IOG accountable to deliver this data?**

* IOG are custodians of the core tools and processes \(Funding dates & budgets, Ideascale admin, voting chain\). If there is anything that changes in those tools or processes then there is a need for the community to be updated about any data changes
* If core tools and processes can be governed by both IOG and the community and eventually just the community then whoever the governing group of people are to each tool and process would become the custodian and then accountable for ensuring data access to the community

**The need for API or repository based data access**

* Community projects that want to develop on top of this data source will want a way to programmatically stay up to date with changes to the data
* Using an API - If data is hosted behind an API then the community can request data at anytime and stay up to date
* Using a repository - If data is stored in a Git repository then the community can get updated by using continuous integration based off of changes to the repository

**Data source required - Fund data**

* **What data** - Fund name, challenges \(name, budget, description, challenge brief\), stages \(name, start and finish times\).
* **Time requirement** - 3-4 hours each fund.
* **Data example:**

```javascript
{
    name: 'Fund 5',
    stages: [
        {
            name: 'Insight sharing',
            startAt: '2021-09-01T12:00:00.000Z',
            finishAt: '2021-09-08T12:00:00.000Z'
        }, 
        ...
    ]
    challenges: [
        {
            name: 'Developer ecosystem',
            budget: '600000'
            budgetCurrency: 'USD',
            description: 'How can we create a positive developer experience that helps the developer focus on building successful apps?'
            ...
        },
        ...
    ]
}
```

* **Current solution** - A community project currently has aggregated together some of this data \([https://airtable.com/shrwVrE8lgcJYOrx0](https://airtable.com/shrwVrE8lgcJYOrx0)\) that is updated by Marek from IOG. The issues currently is this solution is not endorsed by IOG to the wider community and IOG provides no guarantees towards the data accuracy \(it was originally community aggregated data\).
* **Potential solution** - IOG already have to create this data each fund to add to Ideascale and other sources. IOG could go through this existing community project and confirm, add or update all the historical data with the right naming and dates. Once this is done IOG can endorse it as an accurate data source to the community. IOG may want to take full ownership of this due to its importance so they can endorse it and make sure the data concerns only this specific information. The data can also be automatically exported as JSON to a Git repository so the community doesn't need to interact with Airtable.

**Data source required - Ideascale data**

* **What data** - Everything on Ideascale. Personally identifiable information such as emails shouldn't be included.
* **Time requirement** - Time is required up front for final checks on the data that is revealed and on any terms of service legal concerns but afterwards there shouldn't be ongoing requirement.
* **Current solution** - No access. The community needs to scrape Ideascale, copy data manually or get Marek to run a script to access data.
* **Potential solution** - Open up the Ideascale API. Providing no sensitive data is provided this would be the easiest way to provide data access to the community.

**Data source required - Proposal assessment data**

* **What data** - Community advisor assessments, flagged reviews from proposers and vCA responses
* **Time requirement** - A similar usage of time would be used than what is currently being done to add data to the community advisor / vCA tools.
* **Current solution** - Marek from IOG runs a given script for specific community projects. The issue here is the data is not pushed into a data source that the community uses and instead is being pushed into specific solutions. As a result the data is not freely available and endorsed by IOG for the community to use.
* **Potential solution** - A script can still be run however instead the data should be exported as JSON into a data repository. IOG can endorse the data in this repository and highlight the process carried out to generate the data.

**Data source required - Voting data**

* **What data** - Voting results data after snapshot is taking at the end of voting.
* **Time requirement** - IOG already aggregates this data together to make reports. An extra 2 hours is likely needed to turn this into a JSON format and push to an open data repository.
* **Current solution** - Currently only PDF reports are made that highlight the voting result data.
* **Potential solution** - Format the same voting result data into JSON format and push to an open data repository.

**When should this be delivered?**

As soon as feasibly possible. Without alternative solutions the more the user load and stress will be placed onto the existing tools and processes - which haven't been designed to handle a growing ecosystem. The longer the community has with this data the more deliberate and calculated the community can be on improving the process and tools without needing to make any knee jerk ultimatum decisions on changing a tool or process due to it breaking.

**Requirements for delivery**

* **Endorsed** - The custodian of core tools and processes \(IOG currently\) needs to endorse the data source solution they adopt to keep the community aware.
* **Maintained** - The custodian of a process or tool is tasked with maintaining the data source.
* **Accountability** - The custodian of a process or tool is accountable to ensuring the correctness of a data source and for updating anything required to keep it accurate.

**Summary**

IOG are in most cases already creating or extracting the data that is required but what they are not doing is making open accurate data sources for the community. To create a low friction development environment for the community the Catalyst data should standardised and incorporated as part into each process for Catalyst. The better this data is provider the easier it is for anyone in the community to create their own alternative solutions and push the Catalyst ecosystem forward.

