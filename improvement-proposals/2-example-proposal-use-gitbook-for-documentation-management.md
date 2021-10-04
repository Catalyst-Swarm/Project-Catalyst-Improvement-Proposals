# \#2 - Draft Proposal - Use GitBook for documentation management

### **Problem‌**

Project Catalyst is complex. Currently there is a lack of aggregated easy to access quality resources on how the ecosystem works**‌**

### **Solution‌**

Use GitBook to bring together resources into a single location that both IOHK and the community can manage

### **Vote‌**

[**https://forms.gle/XjYMCrtARzgfu6MC9**](https://forms.gle/XjYMCrtARzgfu6MC9)**‌**

## **Research and analysis**

**What this proposal is about**

* Finding and selecting a suitable tool to use for documentation management

**What this proposal isn't about**

* How that tool should be governed and budgeted for
* Who should host the tool

**Why documentation is important**

* Resources help quickly educate people about the Project Catalyst ecosystem who are new to the community and also help existing members keep up to date
* Project Catalyst is complex making documentation more highly valuable to understand how it works
* Project Catalyst has a moderately high rate of change meaning it is easy to lose track of how the ecosystem works at the present moment

**Benefits of quality resources in a single location**

* Clarity & simplicity - Easier to find and track information, clearer to understand the ecosystem
* Simple management - Simple system and process makes resources easier to manage
* Consistency - Consistency on how documentation is created and maintained reduces the chances for confusion, the consistency of a single location makes it easier to share around
* Translations - A stronger base of documentation makes it easier for translations to be created based upon the original documentation

**Problems - IOHK documentation process**

* No single resource location - difficult to track information and updates
* Social posts, messages and emails get lost over time - bad for information management
* Lack of consistency - Documentation is often found in different services \(Google Docs, Reddit, Zendesk\)

**Problems - Community tools**

* Constant follow the leader - Community is constantly playing catch up copying links or information from resources IOHK create into tools. Effort is fragmented.
* Fragile tooling - Community hasn't created tooling that cater for all the requirements of quality documentation management
* Fragmented effort - The community and IOHK aren't effectively learning on the best way to distribute the management of documentation resources

**Catalyst Circle governance comparison**

Catalyst Circle is a good example of distributed governance shared by both IOHK and the community. It makes a good step towards sharing governance with the community in the short term before handing it over in the future when the processes and tools are in place**‌**

Documentation management can follow a similar approach of having both combined IOHK and community governance to create and maintain that documentation**‌**

**Tool requirements**

* Editing interface - Non developer friendly editor to easily manage the resources
* Supports nested structure, formatting & media - Supports nested documents \(pages within pages\), some basic text formatting or styling and handles media content.
* Open source - Anyone should be able to fork the code or copy the data easily, ideally avoid data in centralised databases
* Translations - Support for different languages in the near future
* Multiple contributors & permissions - Both IOHK and the community should be able to manage the resources with multiple contributors with at least a simple permission layer

**Solution options**

Numerous different ways to manage content including documentation tools \(Notion, Gooe Docs, Tettra, Confluence\), Git based documentation \(GitBook, GitHub Pages, Docusaurus\), Git based CMS \(Forestry, NetlifyCMS, Tina CMS\), API based CMS \(Contenful, GraphCMS\) or a custom solution made by the community**‌**

Notes on the tools considered:[ https://tech-notes.notion.site/Documentation-content-management-tools-32425b4c45d043ae98cf12abeb919246](https://tech-notes.notion.site/Documentation-content-management-tools-32425b4c45d043ae98cf12abeb919246)

**Top solutions compared**

![](https://lh4.googleusercontent.com/PXMkv_chCAhNmE1eCFBuW13Z6UsuuUAPrmy1NIESBVa5p5NgvEKDP8dScdmV1hOr3fHKuor_Ea3QSCf2oRpR3_oNos_NEz_aBXJneeDRo_Sf_FMyKKv3AtYn6GGmGqUULr8qVxaX=s0)

**GitBook**

* Editing interface - Has easy to use interface for anyone managing the resources
* Nested structure, formatting & media - Handles one level of nesting into groups, formatting of pages and font styles and can handle media content
* Open source - Easy for entire data structure and any GitBook config to be open source on a repository and data can easily be copied from the repository or the site itself.
* Translations - Yes has translations ability that offers a good experience \([https://docs.gitbook.com/features/internationalization](https://docs.gitbook.com/features/internationalization)\)
* Multiple contributors and permissions - Can have multiple collaborators working with the live interface and has a simple level of permissions available for IOHK to transition control to people

**Notion**

* Editing interface - Has easy to use interface for anyone managing the resources
* Nested structure, formatting & media - Handles multiple levels of nesting into groups, formatting of pages and font styles and can handle media content
* Open source - Data is stored on centralised servers though the data is public so could be copied across. Main issue is the owner of the document could easily change the permissions at anytime and it is also hard to automate regular extraction from the resources without it being in somewhere such as a open source git based system that is easy to have continuous integration on changes to any of the resources.
* Translations - Doesn’t offer any translation tools
* Multiple contributors and permissions - Can have multiple collaborators working with the live interface and has a simple level of permissions available for IOHK to transition control to people

**Google Docs**

* Editing interface - Has easy to use interface for anyone managing the resources
* Nested structure, formatting & media - Doesn’t do nesting of documents well as requires links, formatting of pages and font styles is there and and also can handle media content
* Open source - Data is stored on centralised servers though the data is public so could be copied across. Main issue is the owner of the document could easily change the permissions at anytime and it is also hard to automate regular extraction from the resources without it being in somewhere such as a open source git based system that is easy to have continuous integration on changes to any of the resources.
* Translations - You can auto translate a document in Google Docs but this creates a new document that would need to be linked to making the structure and experience less than ideal.
* Multiple contributors and permissions - Can have multiple collaborators working with the live interface and has a simple level of permissions available for IOHK to transition control to people.

**Community made**

* Editing interface - Current solutions require developers to commit changes, document editing tools would require time to build
* Nested structure, formatting & media - Would require development work, especially if keeping the document information in a simple format like markdown and then parsing that to render on a website with formatting and media content.
* Open source - Can be open source from day one of development.
* Translations - Would require a moderate amount of development work.
* Multiple contributors and permissions - Would require a moderate amount of development work**‌**

**GitBook as a solution**

[resources.projectcatalyst.org](https://resources.projectcatalyst.org/) - Demo of how GitBook could be used

* Custom solution not essential now - Governance and distributed decision making are more important areas of focus than the tooling for resource management. We can use an existing tool like GitBook to help us learn about the governance and distributed management needed for a custom solution in the future.
* Available immediately - Easy to setup and can start using now.
* Low risk permission control - IOHK can control it fully or add community members immediately to help distribute workload
* Production ready - Very popular solution used across many industries
* Better open source solution - Anyone in the community can fork the repository and can also make pull requests to suggest changes
* Easier to integrate - Existing community tools can parse the markdown files and integrate the resources however they want into their tools
* Translations - GitBook allows variants so you can add translations when we’re ready
* Accountable & tracked - All changes are tracked in Git!

Example Cardano projects already using GitBook -[ Minswap](https://docs.minswap.org/faq/fiso),[ Meld](https://meld.gitbook.io/meld/),[ Liqwid](https://liqwid-labs.gitbook.io/liqwid-docs/),[ Catalyst Circle](https://catalyst-swarm.gitbook.io/catalyst-circle/),[ Catalyst School](https://catalyst-swarm.gitbook.io/the-catalyst-school/),[ Catalyst Swarm](https://catalyst-swarm.gitbook.io/catalyst-swarm-genesis/)**‌**

**Problems solved using GitBook**

* Single resource location - Has all the benefits mentioned earlier of clarity & simplicity, simple management and consistency
* Prevents information loss - Prevents what currently happens when social posts, messages and emails are used to share important information
* Better for integration - Provides easier integration for community tools as they can easily link to or parse the markdown files to use them as they want

**Problems solved when GitBook is used with IOHK + Community shared governance**

* Distributed management - Helps with spreading out the responsibility of managing resources
* Faster learning - Helps us learn what is required to manage resources in a distributed way that will inform improvements to the tooling and process over time

**The ideal future - Education**

* IOHK and the community managing the resources will provide experience that guides what governance and tools work well
* Trial tools such as[ canny.io](https://canny.io/) to experiment with ways to get more regular feedback from the community for managing the resources - Determine what is effective or not?
* Different budgeting approaches can be explored \(bounties, hourly rates, part time work\) to determine what’s most effective

**The ideal future - Improve implementation**

* Encourage existing tools like GitBook to integrate identity and governance functionality with Atala Prism - Helps prevents us reinventing the wheel!
* If no existing tool wants to integrate Atala Prism then the community and IOHK are well informed on what type of tooling, governance and budgeting is needed for a custom solution

## **Resources**

* [Presentation video](https://www.youtube.com/watch?v=QNN8PceQuqE) - A presentation on the content shown above
  * [Presentation slides](https://docs.google.com/presentation/d/1S0jFAt9qJWSpbIJ1JiQywS8mJnZFKB14Xd_0HQZZ7w0) - The slides used for the presentation video
* [resources.projectcatalyst.org](https://resources.projectcatalyst.org/) - GitBook demo
* [https://tech-notes.notion.site/Documentation-content-management-tools-32425b4c45d043ae98cf12abeb919246](https://tech-notes.notion.site/Documentation-content-management-tools-32425b4c45d043ae98cf12abeb919246) - Tools considered for this change

