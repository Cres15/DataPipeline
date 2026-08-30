# DataPipeline

SQLite

•Role and ETL Contribution: a serverless and self-contained SQL database that stores data in a local file. In the ETL process, it is mainly used during the Load phase, where the processed data is stored locally for use by the system.   

•Advantages: SQLite is highly portable and does not require a separate backend server or complicated configuration. It supports standard SQL queries and ACID-compliant transactions, making it useful for simple and fast system development.

•Trade-offs: SQLite is not designed for distributed systems or applications with many simultaneous write operations. Its performance may be affected when multiple users or tasks try to update the database at the same time.
