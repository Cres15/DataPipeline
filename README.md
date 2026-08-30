Apache Airflow
Role & ETL Contribution: The Python based orchestrator that acts as the centralized command hub for time based batch workflows. It does not process the data itself, but strictly manages the schedule, coordinates the sequence of the extraction and loading phases, and ensures task dependencies are met.
Advantages: The advantage of apache airflow is that it allows the pipelines to be defined entirely as code using Directed Acyclic Graphs (DAGs), enabling strong version control while providing automatic retries and SLA monitoring out of the box.
Trade-offs: Setting it up requires dedicated backend infrastructure to host its web server and scheduler, which introduces operational complexity.

Python
Role & ETL Contribution: The foundational programming language utilized to execute the Extract phase. It serves as the engine that interfaces with external web sources, APIs, or local directories to pull down the raw batches of files before transformation begins.
Advantages: This advantage is the features of highly readable syntax and a massive ecosystem of specialized libraries, making API connections, file handling, and custom extraction logic straightforward.
Trade-offs: The script execution can be slower than in compiled languages, and managing virtual environments and package dependencies requires strict code organization. 
