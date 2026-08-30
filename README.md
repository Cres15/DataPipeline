Jupyter Notebook & Matplotlib
- Role & ETL Contribution: An interactive development environment and visualization toolkit. While not used in the automated production run, they serve as the crucial Development layer where the pipeline's extraction and loading logic is prototyped and visually validated.
-	Advantages: Enables step-by-step code execution and immediate visual feedback through charts, allowing you to instantly spot errors and verify data integrity before handing the workflow over to Airflow.
-	Trade-offs: Notebook files are inherently difficult to automate or version control, meaning all proven logic must eventually be migrated into standard Python scripts for the final pipeline.
