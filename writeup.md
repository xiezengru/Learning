# Week 2 Write-up
Tip: To preview this markdown file
- On Mac, press `Command (⌘) + Shift + V`
- On Windows/Linux, press `Ctrl + Shift + V`

## INSTRUCTIONS

Fill out all of the `TODO`s in this file.

## SUBMISSION DETAILS

Name: **TODO** \
SUNet ID: **TODO** \
Citations: **TODO**

This assignment took me about **TODO** hours to do. 


## YOUR RESPONSES
For each exercise, please include what prompts you used to generate the answer, in addition to the location of the generated response. Make sure to clearly add comments in your code documenting which parts are generated.

### Exercise 1: Scaffold a New Feature
Prompt: 
```
背景
项目是 Week 2 的 Action Item Extractor：FastAPI + SQLite，把自由文本笔记抽成可勾选的行动项。

请先阅读

week2/app/services/extract.py 里的 extract_action_items(text: str) -> List[str]：用规则（项目符号、关键词前缀、复选框、无匹配时的祈使句启发式等）抽取行动项。
任务
在同一文件（或保持与现有模块风格一致的位置）实现 extract_action_items_llm(text: str) -> List[str]：用 Ollama 调用大模型完成行动项抽取，作为规则版 extract_action_items 的 LLM 替代方案。

技术要求

输出类型与 extract_action_items 一致：List[str]，每项是一条清晰、可执行的行动项字符串。
使用 Ollama 的 结构化输出，让模型返回 JSON 数组（字符串列表），避免手写脆弱解析；参考：https://ollama.com/blog/structured-outputs
模型从 Ollama 库选择即可：https://ollama.com/library；优先选较小模型以降低资源占用；本地拉取/运行：ollama run {MODEL_NAME}
与现有代码风格一致：类型注解、导入方式、错误与边界情况（空字符串、无行动项等）要有合理行为。
在新增/修改处加简短注释，说明为何用 LLM、用的模型名/配置方式（若适合用环境变量，与项目里已有 dotenv 用法保持一致）。
不要做

不要改作业范围外的 large refactor（TODO 3 单独做）。
若已有 extract_action_items，保留它；只新增 extract_action_items_llm 及 Ollama 调用所需的最小依赖与配置。
``` 

Generated Code Snippets:
```
extract.py
Lines 71-139
```

### Exercise 2: Add Unit Tests
Prompt: 
```
Write unit tests for `extract_action_items_llm()` covering multiple inputs (e.g., bullet lists, keyword-prefixed lines, empty input) in `week2/tests/test_extract.py`.
``` 

Generated Code Snippets:
```
test_extract.py 1-14; 30-145
```

### Exercise 3: Refactor Existing Code for Clarity
Prompt: 
```
 Refactor the backend code of week2 with focus on:
1. 
API Contracts - Define clear Pydantic request/response schemas, consolidate validation logic
2. 
Database Layer - Clean up session management, abstract queries into repository pattern, add proper transactions
3. 
App Lifecycle - Centralize config loading, structured startup/shutdown events, health checks
4. 
Error Handling - Unified exception hierarchy, consistent HTTP error responses, proper logging

Please read current implement first.
Then think about the plan of refactor.
Refract the code step by step.

Keep existing functionality. Add tests for refactored components.
``` 

Generated/Modified Code Snippets:
```
TODO: List all modified code files with the relevant line numbers. (We anticipate there may be multiple scattered changes here – just produce as comprehensive of a list as you can.)
```


### Exercise 4: Use Agentic Mode to Automate a Small Task
Prompt: 
```
TODO
``` 

Generated Code Snippets:
```
TODO: List all modified code files with the relevant line numbers.
```


### Exercise 5: Generate a README from the Codebase
Prompt: 
```
TODO
``` 

Generated Code Snippets:
```
TODO: List all modified code files with the relevant line numbers.
```


## SUBMISSION INSTRUCTIONS
1. Hit a `Command (⌘) + F` (or `Ctrl + F`) to find any remaining `TODO`s in this file. If no results are found, congratulations – you've completed all required fields. 
2. Make sure you have all changes pushed to your remote repository for grading.
3. Submit via Gradescope. 