## ChatGPT project

requirment: interactive feedback involved cycle, easy to understand close to natural language but accurate executables.


In threat detection process, the amount of invovled knowledge, information and data are huge.
These includes threat inteligence TTPs, local context of risks and vonulbilitys,
 log, configuration and deployment files, software version/patchs, assets, application and network enclaves in attack chain,
and the dynamic characteristics of new threat intelligence reports.

GPT modele can provide an ideal solution by consolidating this huge amoung of knowledge and information,
and interactively direve to the final result with feedbacks prompts incorporateing the local relevent context.
With GPT modle as the core, the developed security platform can quickly 
acomplish the convergence and generate executable playboods and automations as the final output.
Compare with other security products, the platform backed by GPT model equipted by a huge knowledge base, an updated
threat intelegence and natural language interface can provide security expert the cutomized tools for threat detectiona
and remidation.

The result gnerated from GPT model for interactively refinement should be easy to understand, accurate and executable.
We will use a declarative language to capture the output from the GPT model. 

KiwiSpec is declarative language designed for accessing json-formated log/configuration data set for data manipulation,
aggregation, transformation and constrain validation. 

As a declarative language, KiwiSpec closely resembles natural language but with accurate semantics. 
Specifications written in KiwiSpec are easy to adopt, read, maintain, and are unambiguous.


While GPT model can generate code in languages like Python, C, SQL, and others, 
KiwiSpec is selected as the interface bacuse it would be closer to 
describ the original request and easier to understand, proofread, and modify the generated code.

## Asset discory platform
A kiwi-analitical is an interactiv platform for user to discover their envioronment by natural language quries. 
The platform provides user the capability to explore their envioronment for assets, applications, activites, dependencies, 
vonerablities, violations and attack pathes. 
During exploration, user can inquire the platform Empowered by GPT for the knowledge of networking, cloud, security 
and threat intelegence and incorperate the knowledge into the exploration process.


The platform is build from Kiwispec language and integrated with GPT model. The data source are log files, configuration files, and deployment files in json format.

Users can use natural language to describe what they want to explor,
how they want to classify their assets, what activites they want to exame, 
and the relationship they want to trace along a path.

Users requests are translated to executables in Kiwispec. Kiwispec is a SQL like query language
with the extension of the capabilty to access and query JSON data. 
kiwispec is designed as declarative language for data access, data manipulation, 
knowledge extraction, and constraint validation with json-formated data set.

The platform integrated with GPT model has built in promts and built in best practice rules.
Kiwispec platform supports an interactive interface. User can interactivly
explore and fine tune the cretier 
To get meaningful classification of assets and applications and capture the right baseline of dependency and activites,
Kiwispec platform provides user an interactive interface with test run and result analysis 
during this exploration process for user to fine tune their query cretiera.
The interactive platform allows user to incorperate 
configurations, identities and software updates to explore the vonerabilites and the attack paths.
At anytime during this process, user can consult the platform powered by GPT for 
the knowledge on networking, cloud, security and threat intelegence interactively.

Once the meaningful grouping and baselining are achieved.
The finalized kiwispec can be used at automation to get regular update on the envioronment discovery.
Using the discovered relationship，
the platform allows user to create permitted traffic rules and deploy the validation checking 
for future activies.
