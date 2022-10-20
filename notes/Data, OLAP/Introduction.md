## Heterogeneous Data Sources
- **Broad range of data sources**
	- database systems(relational, object-relational, XML,..)
	- Enterprise Resource Palnning Systems (ERP)
	- external information sources (other companies, surveys, ...)
	- files (Excel, ...)
	- other documents (Word, WWW, ...)
- **Data Sources may differ in**
	- schema
	- coding schemes
	- time frame (when is data sent)
	- treatment of history
	- aggregation level (in which time frames is data stored)
	- DBMS (data model, vendor, version)
	  
## Data Warehouse
![[DataWarehouse.png]]

### Operational vs. Analytical Systems
![[OperationalVsAnalyticalSystems.png]]
### Important Terms
- **Data Warehousing**
  **Process of integrating data from several source systems, storing it in the data warehouse
  database, and using this integrated data source.**
  
- **Business Intelligence**
  **General term that covers technology and tools to turn the volume of data an organization collects and stores into meaningful information in order to achieve better and timelier business decisions.**

- **Decision Support**
  **More general term referring to all kinds of analyses of existing data in order to make better decisions - like data mining, online analytic processing (OLAP), simulation, scenario analyses, ...**
  
#### Fields of Application
- **Business management**
	- marketing
	- enterprise information portals
	- Customer Relationship Management (CRM)
	- supply chain management
- **Scientific applications**
	- empirical studies, e.g. erath observation, enviromental studies
	- statistical and scientific databases (SSDB)
- **Engineering applications**
	- analyzing the reliability of products
	- analyzing substances and material
	  
## Introduction to Services
- A **repeatable business task** - e.g. check customer credit, open new account
- Discretely defined **set** of contiguous and autonomous business or technical **functionality**
- A **function** provided at a network address
- A mechanism to enable access to capabilities, which is
  provided using a prescribed interface and is exercised consistent with constraints and
  policies as specified by the service description
## Introduction to SOA
![[SOA.png]]
- An **IT architectural style** that supports integrating your **business as linked services**
- A method for systems development and integration where functionality is grouped
around business processes and packaged as interoperable services
- An architectural style to realize service-oriented computing
- A paradigm for organizing and utilizing distributed capabilities that may be under
the control of different ownership domains
## Information Services
- **Service-oriented Architecture**
  >You will waste your investment in SOA unless you have enterprise information that SOA can exploit." (Gartner, 2005)

- **Information Service**
	- **Definition:** Every capability needed to understand, cleanse, integrate and deliver information across heterogeneous systems
	-  **Is:** Data Storage + Retrieval (and crunching)
	- **Goal:** services that provide ==accurate, consistent, integrated information== to business processes and people
	- **Starting point:** existing legacy, inconsistent & divers data
	- **Approach for Information as a Service**
		- Exposing application logic as services
		- Data is only accessible trough the corresponding application logic
		- If needed: Mediation (brokering) and archestration (workflow) of application logic

- **Classification Criteria**
	- Level of abstraction
		- Plain source data (SQL, ..) or meta data
		- Integrated data (data/information integration, ETL,...)
		- Interpreted data (BI, text analytics, contents extraction)
		- Application data (CRM, ..)
	- Range
		- Intranet
		- Internet
	- Source
		- Single or multiple sources
		- Homogeneous or heterogeneous
	- Provisioning of the service
		- Proprietary service
		- Web/SOA service
## Cloud Computing
>“Cloud Computing is a style of computing where massive scalable IT-enabled capabilities are delivered as a service to external customers using Internet technologies.” (Gartner)

- **Business properties of Cloud Computing**
	- No startup (hardware) cost
	- Pay per use
- **Technical Properties**
	- simple, easy programming model
	- scalability, reliability, administration easy possible
	- Minimum TCO -> Autonomic/Cloud, Multi-tenancy
	![[CloudComputing.png]]