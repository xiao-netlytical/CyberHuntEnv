
<img width="166" alt="Screen Shot 2024-02-22 at 2 31 51 PM" src="https://github.com/xiao-netlytical/CyberHuntEnv/assets/128750656/e2efd6aa-27b6-4685-b7d7-20b97fe1d179">


CyberHuntEnv is an open-source project and platform dedicated to creating an environment for IT and security professionals. It empowers them to comprehend their dynamically evolving environments, establish baselines, identify anomalies, and implement security measures.
     
xiao.netlytical@gmail.com  

## CyberHuntEnv

CyberHuntingEnv is an interactive platform designed to enable users to understand their environments, identify vulnerabilities, establish baselines, detect anomalies and potential attacks, and enforce security measures.

The platform enables users to explore their environments using natural language queries, accessing a comprehensive dataset encompassing logs, configurations, deployments, and captured files.

Users have the capability to investigate various aspects of their environments, including assets, applications, activities, software versions, relationships, dependencies, and logical constraints.

CyberHuntingEnv seamlessly integrates with generative AI. During exploration, users can leverage AI models' extensive knowledge on operating systems, networking, cloud computing, threat intelligence, and MITRE ATT&CK TTPs.

Through the interactive interface, users can execute and refine their explorations, analyze results, and build aggregated databases. This iterative exploration process enables users to gain deeper insights into their environments.

## Empowered by LLM model

In the realm of cybersecurity and threat hunting, the volume of knowledge, information, and datasets involved is substantial. These encompass:

1. Knowledge of operating systems, protocols, networking, and cloud environments.
2. Threat intelligence Tactics, Techniques, and Procedures (TTPs).
3. Discovered local environments of assets, applications, dependencies, and network enclaves.
4. Collected logs, configurations, and deployment files, including software versions and patches.
5. Local context regarding risks, vulnerabilities, and attack patches.
6. Dynamic characteristics of new threat intelligence reports.

CyberHuntEnv, serving as an LLM agent with RAG and empowered by an LLM model, offers users an ideal solution with a consolidated knowledge base featuring updated threat intelligence and a natural language interface.

As users develop their exploration plans and formulate queries, they can interactively consult the platform for information and knowledge. The platform enables users to progressively acquire information starting from high-level requests and drilling down to technical details associated with data files, including format, fields, and values.  Additionally, the platform will refine user's queries with the aid of predefined prompts and prompt chains, guiding them to obtain the desired details.

The GPT model comprehends natural language queries from users and delivers precise and executable outputs in a declarative language—KiwiSpec.

Through continuous learning and enhancement of prompt chains, we anticipate that the GPT model will comprehend very high-level queries, integrate extensive domain knowledge, address any gaps, and generate executable KiwiSpec outputs. One of the ultimate goals will be deriving the executable KiwiSpecs from a threat intelligence report.

## Empowered by KiwiSpec
https://github.com/xiao-netlytical/KiwiSpec

Utilizing log files, configuration files, and deployment files in JSON format as input sources, users can specify the assets and contents they wish to extract, classify assets, examine activities and dependencies, establish baselines, and track relationships.

CyberHuntingEnv, powered by GPT and KiwiSpec, interprets natural language inputs regarding the above requests, and translates them into executable outputs with accurate semantics and user-friendly language. This language feature facilitates user proofreading and query refinement.

KiwiSpec, akin to a SQL query language but tailored for JSON-formatted datasets, enables declarative data access, manipulation, information extraction, and constraint validation. It excels in data manipulation tasks such as aggregation, correlation, transformation, information extraction, and constraint validation.

Specifications written in KiwiSpec closely resemble natural language but offer precise semantics, making them easy to adopt, read, maintain, and without ambiguous. 

While the GPT model can generate executable solutions in languages like Python, C, and SQL, KiwiSpec serves as an output interface closer to the original request, facilitating better understanding, proofreading, and modification.

## Recursive Exploration

The advantage of this platform lies in its interactive functionality, enabling recursive exploration cycles. Users start with natural language queries, receive confirmation feedback from the AI model with accurate semantics, engage in proofreading and editing, and conduct test runs.

This unique design empowers users to iteratively create new transformed datasets through aggregation and correlation. Within the hypothesis/execution cycle, users can develop a series of queries to gradually uncover insights from the dataset. Notably, intermittent datasets become part of the input dataset for subsequent query cycles. This process also facilitates prompt chain learning and development to enhance the platform.

During exploration exercises, users can fine-tune their queries through test runs and result analysis to achieve meaningful classification and aggregation of assets, establish appropriate baselines for dependencies and activities. Once meaningful classification, aggregation, and baselines are attained, the finalized KiwiSpec can be used for ongoing validation through automation. Additionally, security rules can be derived to identify anomalies, outliers, and violations.

## Other Features and Details

The platform enables users to:

Create and store transformed datasets derived from abstractions and aggregations.

Selectively record interactions, including query prompts, KiwiSpecs, and resulting datasets.

Collect KiwiSpecs as discovery rules for ongoing discoveries.

Collect KiwiSpecs as security validation rules for ongoing validations.

Launch the platform with pre-built prompts and pre-built KiwiSpecs.

Continuously learn new prompts, prompt chains, and KiwiSpecs.

Generate discovery and violation reports.

