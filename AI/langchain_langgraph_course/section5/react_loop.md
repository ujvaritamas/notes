# React loop
LLM decides which tools to call, then calls the selected tools and saves the results to the messages list.
AI message -> it defines what tools are selected for execution.
ToolMessages contain the results of the called tools.

If the final AI message did not contain selected tools, then no more tool selected, and the final response was created by the LLM.

Every time when llm is called, it has access to what was performed in the past. If there are no more tool calls, it means that the final answer has been created.
