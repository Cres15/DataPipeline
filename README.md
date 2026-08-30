Jupyter Notebook & Matplotlib
- Role & ETL Contribution: An interactive development environment and visualization toolkit. While not used in the automated production run, they serve as the crucial Development layer where the pipeline's extraction and loading logic is prototyped and visually validated.
-	Advantages: Enables step-by-step code execution and immediate visual feedback through charts, allowing you to instantly spot errors and verify data integrity before handing the workflow over to Airflow.
-	Trade-offs: Notebook files are inherently difficult to automate or version control, meaning all proven logic must eventually be migrated into standard Python scripts for the final pipeline.
Apache Airflow
Role & ETL Contribution: The Python based orchestrator that acts as the centralized command hub for time based batch workflows. It does not process the data itself, but strictly manages the schedule, coordinates the sequence of the extraction and loading phases, and ensures task dependencies are met.
Advantages: The advantage of apache airflow is that it allows the pipelines to be defined entirely as code using Directed Acyclic Graphs (DAGs), enabling strong version control while providing automatic retries and SLA monitoring out of the box.
Trade-offs: Setting it up requires dedicated backend infrastructure to host its web server and scheduler, which introduces operational complexity.

Python
Role & ETL Contribution: The foundational programming language utilized to execute the Extract phase. It serves as the engine that interfaces with external web sources, APIs, or local directories to pull down the raw batches of files before transformation begins.
Advantages: This advantage is the features of highly readable syntax and a massive ecosystem of specialized libraries, making API connections, file handling, and custom extraction logic straightforward.
Trade-offs: The script execution can be slower than in compiled languages, and managing virtual environments and package dependencies requires strict code organization. 
