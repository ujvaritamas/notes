# Intro

Framework what can help developers to create AI powered applications.
Same interface for the currently most popular llm vendors.
```
llm = ChatOllama(
    model="llama3.1",
    temperature=0,
    # other params...
)

model = ChatAnthropic(
    model="claude-haiku-4-5-20251001",
    # temperature=,
    # max_tokens=,
    # timeout=,
    # max_retries=,
    # ...
)
```

PromptTemplate (jinja2 can be better)
```
from langchain_core.prompts import PromptTemplate

# Instantiation using from_template (recommended)
prompt = PromptTemplate.from_template("Say {foo}")
prompt.format(foo="bar")

# Instantiation using initializer
prompt = PromptTemplate(template="Say {foo}")
```

Promptemplate similar to f string but it will fail if the corresponding variables not set.

- Langsmith tracing
