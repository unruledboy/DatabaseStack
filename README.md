# DatabaseStack
database technology stack, including MS SQL Server, Azure etc.



# What and why?
Have you ever wondered:
* what technologies database server really includes? 
* how many do I possess?


I could not find a really comprehensive diagram that shows the database technology stack, so I come up with my own version.

There might be issues here and there, like the category, the individual ones, but the beautity is you can modify it as you want.



# The Database Stack

You can have a graphical preview here: https://rawgit.com/unruledboy/DatabaseStack/master/ux/DatabaseStack.htm 


- RDBMS
	- MS SQL Server
		- SQL OS
			- Memory Management
			- Buffer Pool
			- Deadlock detection
			- Exception handling
			- Schedulers
			- InterOp
		- Storage Engine
			- Transaction Services
			- File Manager
			- Data File
			- Extents
			- Pages
			- Log File
				- Write Ahead
		- Relational Engine
			- Query Processing
				- Parser
				- Optimizer
				- SQL Manager
				- Database Manager
				- Query Executor
			- Memory Management
			- Thread and Task Management
			- Buffer Management
			- Distributed Query Processing
		- Communication 
			- Tabular Data Stream (TDS)
			- Protocols
				- TCP/IP
				- Named pipes
				- Shared memory
				- Web Services
		- Core Concepts
			- Instance
				- Default
				- Named
			- Port
				- Default: 1433
				- Dynamic
			- Transaction
				- ACID
					- Atomic
					- Consitent
					- Isolated
					- Durable
				- Checkpoint
				- Isolation Levels
					- Read uncommitted
					- Read committed
					- Repeatable read
					- Snapshot
					- Serializable
			- Concurrency
				- Lock
					- Optimistic
					- Pessimistic
					- Exclusive
					- Shared
				- Wait
				- Latch
				- Deadlock
					- Kill
				- sync/async
				- Blocking
				- Row versioning
		- Core Objects
			- Database
				- Recovery model
					- Simple
					- Full
					- Bulk logged
				- Compatibility level
					- 130: SQL  Server 2016
					- 120: SQL  Server 2014
					- 110: SQL  Server 2012
					- 100: SQL  Server 2008
					- 90: SQL  Server 2005
					- 80: SQL Server 2000
			- Table
				- FileTable
			- View
			- Stored Procedure (SP)
			- Function (FN)
				- Table-valued Function
				- Scalar-valued Function
			- Type
				- System Type
				- User-defined Type (UDF)
			- Index
				- Clustered Index
				- Non-clustered Index
			- Column
				- columnstore
				- NTFS FileStream
			- Schema
			- Trigger
				- Table Trigger
					- BEFORE
					- AFTER
					- INSTEADOF
			- Constraint
			- Key
			- Default
			- Assembly
			- Synonym
			- Collation
			- Login
			- User
			- Rule
			- Server role
			- Endpoint
			- Job
			- Cursor 
			- Linked Server
			- Service Broker
		- Standard
			- ANSI 92
		- Languages
			- Query Language
				- T-SQL (Transact-SQL)
				- MDX (MultiDimensional eXpressions)
			- Data Manipulation Language (DML )
				- CRUD
					- Create(INSERT)
					- Retrieve(SELECT)
					- Update
					- Delete
			- Data Definition Language (DDL)
				- CREATE
				- ALTER
				- DROP
				- TRUNCATE
			- Data Control Language (DCL)
				- GRANT
				- REVOKE
			- Transaction Control Language (TCL)
				- BEGIN TRANSACTION
				- COMMIT
				- ROLLBACK
				- SAVE TRANSACTION
		- System database
			- master (dbs, login, configs)
			- tempdb (temp tables / sps)
			- msdb (jobs/alerts/backups)
			- model (template for new db)
			- resource (invisible, system objects) 
		- File
			- primary (MDF)
			- secondary (NDF)
			- log (LDF)
			- File/Filegroup
		- Runtime
			- Process
			- Worker
			- Connection
			- Request
			- Stall
			- Stats
			- Cache
				- aging
			- Catalog Views
			- Dynamic Management Views (DMV)
				- Execution count
				- Execution io/cpu/perf
			- Full Text Search (FTS)
				- Integrated Full Text Search (iFTS)
		- Replication
			- Log Shipping
			- Publish/Subscribe
				- Transactional
				- Merg
				- Snapshot 
			- Mirroring
			- AlwaysOn
			- Clustering
			- Snapshot
		- Versions
			- Express
			- BI
			- Web
			- Standard
			- Enterprise
			- Datacenter
			- Local DB
		- Management
			- SQL Server Management Studio (SSMS)
			- SQL Server Command Line Util (sqlcmd)
			- SQL Monitor ;-)
		- Maintenance
			- Maintenance Plan
			- Logs
			- Database Mail
			- Backup/Restore
				- Mode
					- Full
					- Differential
					- Transaction log
			- Import/Export
			- Shrink
			- DBCC
			- Bulk Load
			- Online/Offline
			- Attach/Dettach
			- Resource governor
			- Facets
		- Business Intelligence (BI)
			- SQL Server Integration Service (SSIS)
			- SQL Server Reporting Service (SSRS)
			- SQL Server Analysis Service (SSAS)
		- Troubleshoot
			- Dedicated Administrator Connection (DAC) - "ADMIN:INSTANCE"
			- SQL Server Profiler
			- Activity Monitor
		- Performance
			- Seek
			- Scan
			- Fragmentation
			- Partitioning
			- Database Engine Tuning Advisor

	- Oracle
	- MySQL
	- PostgreSQL
	- Informix

- Cloud
	- Azure

- NoSQL
	- Azure Document DB
	