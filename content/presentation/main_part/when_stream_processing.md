# When Stream Processing (Intoduction) 

## History of Stream Processing
- More and more popular technology with companies big and small
- Superior solutions for many use cases such data analytics, ETL (Extract, transform and load) and transactional applications
- Facilitates novel application (new solutions new applications ...), software architectures and business opportunities

_cite: Hueske (S. 23)_

### Traditional Data Infrastructures
- Two types of traditional architecutre: *transactional* processing and *analytical* processing

#### Transactional Processing
- Examples of appications used for day-to-day business: ERP (enterprise resource planning), CRM (custom relationship management), web-based applications
- These Systems designed with seperate tiers for data processing (application itself) and data storage (a transactional database system)
- Event &rarr; Response : Example Order Event &rarr; processing by order System connected to Transactional DBMS &rarr; Response / is one service
- Multiple services connected to one database or one table &rarr; causes problems if need to evolve or scale the application (for example if you want to change the schema of a table or database)
- Microservices (doing a single this, but doing it well) &rarr; connectiong microservices via RESTful HTTP / microservices architecture (containers)

_cite: Hueske (S. 24 ff.)_

#### Analytical Processing
- Is stored in various transactional database systems of a company. For example order-data can be analyzed to obtain sales growth over time, to identify readons for delayed shipping, predict future sales (...)
- Data is mostly unique and often distributed across several disconnected database systems
- Data needs to be transformed into a common format
- For analyzing data it needs to be copied (ETL)
- ETL: extract-transform-load extract data from transactional database, transforms it into a common representation that might include validation, value, normalization (...) and finally loads it into the analytical database.
- ETL need to run periodicly, to keep data warehouse synchronized
- ad-hoc (business-critical-decisions) and periodic report queries (reports) &rarr; both executed by a data warehous in a batch processing fashion

_cite: Hueske (S. 27 ff.)_

### Stateful Stream Processing

### A bit of history
- Some of the first research prototypes and commercial products date back to the late 1990s
- Grown by availability of mature open source stream processors and many open source communities
- Open source communities are constantly improving with new features and capabilities
- Today stream processors power business-critical-applications in many enterprises across different industries (gaming, banking, social media ...)
- First distributed open source stream processors (2011) focused on event processing with millisecond latencies and provided guarantees against loss of events in the case of failures
- Had low lvl APIs
- First open source stream processor in contrast to batch processors traded result accuracy for better latency
- At this point in time (first open source stream processor) could either provide fast or accurate results (*lambda architecture*)
- Lambda architecture augments traditional batch processing architecture with a speed-layer that is powered by a low-latency stream prcoessor
- Lambda is not state of art, but still used in many places
- Goal of Lambda was 
- Secont generation of open source processors (2013) 
- Thirs generation of open source processors (2015) 

_cite: Hueske (S. 39 ff.)_
