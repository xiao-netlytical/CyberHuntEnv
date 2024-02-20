
Our objective is to develop an environment for IT and security professionals that facilitates learning about their dynamically evolving environments, establishing baselines, identifying anomalies and outliers, and implementing security measures.

## CyberHuntEnv

CyberHuntingEnv is an interactive platform designed to enable users to understand their environments, identify vulnerabilities, establish baselines, detect anomalies and potential attacks, and enforce security measures.

The platform enables users to explore their environments using natural language queries, accessing a comprehensive dataset encompassing logs, configurations, deployments, and captured files.

Users have the capability to investigate various aspects of their environments, including assets, applications, activities, software versions, relationships, dependencies, and logical constraints.

During exploration, users can leverage the platform's extensive knowledge base on operating systems, networking, cloud computing, security, and threat intelligence, augmented by MITRE ATT&CK techniques.

The platform offers an interactive interface for users to refine and execute their exploration queries, analyze results, and build aggregated databases. This iterative exploration process enables users to gain deeper insights into their environments.

## Empowered by GPT Model

In the realm of cybersecurity and threat hunting, the volume of knowledge, information, and datasets involved is substantial. These encompass:

1. Knowledge of operating systems, protocols, networking, and cloud environments.
2. Threat intelligence Tactics, Techniques, and Procedures (TTPs).
3. Discovered local environments of assets, applications, dependencies, and network enclaves.
4. Collected logs, configurations, and deployment files, including software versions and patches.
5. Local context regarding risks, vulnerabilities, and attack patches.
6. Dynamic characteristics of new threat intelligence reports.

Compared to other security products, the platform, empowered by the GPT model, offers users an ideal solution with a consolidated knowledge base featuring updated threat intelligence and a natural language interface.

As users develop their exploration plans and formulate queries, they can interactively consult the platform for information and knowledge. The platform enables users to progressively acquire information starting from high-level requests and drilling down to technical details associated with data files, including format, fields, and values. 
Additionally, the platform empowers users to refine their queries with the aid of predefined prompts, guiding them to obtain the desired details.

The GPT model comprehends natural language queries from users and delivers precise and executable outputs in KiwiSpec.

*(In the future, we anticipate that the GPT model will comprehend very high-level queries, integrate extensive domain knowledge, address any gaps, and generate precise and executable outputs in KiwiSpec.)*

## Empowered by KiwiSpec

Utilizing log files, configuration files, and deployment files in JSON format as input sources, users can specify the content and assets they wish to extract, classify assets, examine activities and dependencies, establish baselines, and track relationships.

The CyberHuntingEnv, powered by GPT and KiwiSpec, can interpret natural language inputs and translate them into executable outputs with accurate semantics and user-friendly language. This language facilitates user proofreading and query refinement.

KiwiSpec, akin to a SQL query language but tailored for JSON-formatted datasets, enables declarative data access, manipulation, information extraction, and constraint validation. It excels in data manipulation tasks such as aggregation, correlation, transformation, information extraction, and constraint validation.

Specifications written in KiwiSpec closely resemble natural language but offer precise semantics, making them easy to adopt, read, maintain, and without ambiguous. 

While the GPT model can generate executable solutions in languages like Python, C, and SQL, KiwiSpec serves as an output interface closer to the original request, facilitating understanding, proofreading, and modification.

## Recursive Exploration

The advantage of this platform lies in its interactive functionality, which follows an exploration cycle—from natural language query to accurate confirmation feedback, to proofreading and editing, to test runs.

This unique design empowers users to iteratively create new transformed datasets through aggregation and correlation. Users can develop a series of queries within the hypothesis/execution cycle to gradually uncover the underlying factors of the dataset. Notably, the intermittent datasets become part of the input dataset for the subsequent query cycle.

During the exploration exercise, users can fine-tune their queries through test runs and result analysis to achieve meaningful classification and aggregation of assets, establishing the appropriate baseline for dependencies and activities. Once meaningful classification, aggregation, and baselines are attained, the finalized KiwiSpec can be utilized for ongoing validation through automation. Additionally, security rules can be derived to identify anomalies, outliers, and violations.

## Other Features

Users can create and store new transformed datasets derived from abstractions and aggregations.

The platform enables users to selectively record interactions, including prompts, KiwiSpec queries, and resulting datasets.

Collected KiwiSpecs can serve as security validation rules.

The platform is launched with pre-built prompts and pre-built KiwiSpecs.

The platform offers report generation, best practices and security rule generation.

### Features:

- Browse built-in KiwiSpecs
- Browse pre-built prompts
- Run KiwiSpec queries to examine outputs
- Save running outputs as datasets
- Save prompts as built-in prompts
- Save KiwiSpec queries as built-in specifications
- Document the exploration process

### Stages:

1. Learn environment
2. Discover vulnerabilities
3. Develop baselines
4. Identify anomalies and outliers
5. Create security rules
6. Documenting at any stage

### Flow:

1. Hypothesis development:
   - Prompts for gathering knowledge
   - Prompts for consolidating involved logs and configurations, including format and fields
2. Query planning:
   - Pull in involved logs and configurations: local file locations
3. KiwiSpec generation:
   - Translate natural language query prompts to KiwiSpec queries
   - Edit KiwiSpec queries
4. Test KiwiSpec queries:
   - Go back to step 2 as needed
5. Close one hypothesis:
   - Save selected knowledge, prompts, KiwiSpecs, and outputs
   - Go back to step 1
6. Develop security rules and set up automation

### Result Data Examples:

- Aggregated groups of workloads
- Aggregated traffic patterns
- Cross-referencing applications
- Accessing tracks
- Internet access tracks
- Software versions
- Processes initiated (Event ID 4688), especially those running on only a few machines
- Registry changes (Event ID 4663)
- Task scheduling and task state changes (Event ID 4698 - 4702)
- Addition of unknown/unapproved services (Event ID 4697)
- User additions to privileged groups (Event ID 4728, 4732, 4756)
- Files cleaned except for downloads, such as those in System32
- Instances of `cmd.exe` launched from `winword.exe`
- Instances of `powershell.exe` making outbound connections
- Instances of `svchost.exe` launched from `services.exe`
- Usage of `cscript.exe`, `wscript.exe`, and `powershell.exe`
- Reasons for using `EncodedCommand`
