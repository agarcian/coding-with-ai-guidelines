# Guidelines to effciently write software code with AI assistants

This document contains suggestions and guidelines on how to leverage AI assistants to write software code efficiently.

## Think Localized vs. Comprehensive

When working on software development tasks, selecting the right tool based on the scope of your work is crucial. Tools like GitHub Copilot and Amazon CodeWhisperer (Amazon Q) are particularly effective for generating code within a single file. These tools excel at providing quick, context-aware suggestions that are localized to the specific piece of code you are working on, making them ideal for tasks such as writing functions, completing code snippets, or making small adjustments within a file.

However, when you're creating a new solution, designing a function that spans multiple files, or need to consider the broader context of your project, tools like ChatGPT and Claude can offer significant advantages. These tools allow you to input larger portions of your codebase, including multiple files, and can provide suggestions that consider the overall architecture, dependencies, and interactions within your project.

It’s important to note, though, that while ChatGPT and Claude provide a broader perspective, they may require constant reprompting to maintain context accurately across your codebase. This can be a minor inconvenience, but it doesn’t outweigh the benefit of receiving comprehensive guidance for multi-file projects, architectural decisions, and system-wide design considerations.

By understanding the strengths and limitations of each tool, you can choose the most appropriate one for the task at hand, optimizing both efficiency and the quality of your code.

## Start with a Comprehensive Prompt

When initiating a coding session with an AI assistant, it's crucial to craft a comprehensive initial prompt. This prompt should clearly outline the purpose of the code you intend to write and specify the technologies you wish to use, such as whether you prefer TypeScript over JavaScript or if you're using a specific framework (e.g., "We're using Framework XYZ version 1.0 to build this feature").

Additionally, it's important to describe any dependencies your code will utilize. Define these dependencies by name—for example, "the backend is a REST API named MyBackend" or "the database is PostgreSQL"—as this makes it easier to refer to them in future prompts without needing to re-explain them.

The more detailed and specific your initial prompt is, the better the AI can assist you throughout the session. This comprehensive approach ensures that the AI has all the necessary context from the start, leading to more accurate and relevant code generation and reducing the need for follow-up explanations.

## One Task Per Session
To maintain clarity and improve the quality of AI-generated code, it's essential to focus on one task per session. This means that if you're working on a project with multiple components—such as a frontend, backend API, and data layer—each of these should be handled in separate AI sessions.

By compartmentalizing your work into distinct sessions, you avoid context pollution, ensuring that the AI remains focused on the specific task at hand. This is particularly important when developing different layers of a project in parallel, as it allows you to maintain clear boundaries between components.

For example, if you're developing a backend API and a frontend simultaneously, start separate sessions for each. Once a backend endpoint is completed—such as "MyBackend now supports this new endpoint to handle user authentication"—you can then initiate a new session focused on building the corresponding frontend action. This approach not only keeps your sessions organized but also allows you to efficiently manage dependencies between different parts of your project.

By isolating tasks in this way, you'll find that the AI's assistance is more accurate and contextually appropriate, leading to better overall results.

## Think Step-by-Step

When working on tasks that involve creative problem-solving, such as code architecture or developing new features, it's beneficial to adopt a step-by-step approach. This method not only helps guide the AI through detailed problem analysis but also aligns with best practices in software development, like making small, incremental changes.

Breaking down your work into smaller tasks allows you to maintain greater control over the development process. After the AI generates new code, you can carefully review it by pasting the code into your project and using difference views in your version control system (like Git) to see exactly what has changed. This enables you to selectively integrate the code you find useful while rejecting anything that doesn't meet your standards or expectations.

By working in small increments, you can provide updated context back to the AI in your next prompt, ensuring that the assistant remains aligned with the evolving state of your project. This approach not only fosters better collaboration between you and the AI but also minimizes the risk of introducing errors, leading to a more controlled and reliable development process.

## Update AI with Latest Context

When working with AI assistants, it’s important to recognize that they may not always be up-to-date with the latest versions of frameworks, plugins, or other tools you're using. However, this limitation can be easily addressed by providing the AI with additional context, such as documentation, Swagger files, or snippets of sample code.

If the AI doesn’t have the latest information, simply paste the relevant documentation or example code into your prompt and ask the AI to generate code based on it. This ensures that the code produced aligns with the most current standards and practices.

Additionally, there may be specific preferences or conventions within your project that you want the AI to follow consistently. For instance, you might prefer that the AI always uses Format A instead of Format B when generating code. You can include such instructions in your prompts to guide the AI in maintaining consistency throughout your project.

By keeping the AI updated with the latest context and clearly stating your preferences, you can significantly enhance the relevance and accuracy of the code it generates, making it a more effective tool in your development process.

## Refine by Revisiting Chat History
In the course of using an AI assistant, there may be times when the development process takes an unexpected turn, leading to code or logic that doesn’t meet your needs, or when the AI gets stuck in a loop, providing repetitive or unhelpful suggestions. When this happens, it's important to manage the context effectively to avoid further issues.

One effective strategy is to revisit the chat history and identify the point where things began to diverge from your desired outcome. By updating or editing the prompt at that specific branch, you can reset the context, removing any unhelpful or irrelevant information from the AI’s understanding. This allows you to craft a better prompt that steers the session back on track, avoiding the pollution of context that might have occurred.

By refining the prompt in this way, you ensure that the AI focuses on the correct path, leading to more accurate and useful code generation. This method helps maintain clarity and direction in your sessions, enabling you to make the most of the AI’s capabilities.

## Ask for Comments and Explanations

When working with AI-generated code, it’s highly beneficial to request detailed inline comments. These comments provide valuable explanations of the code, making it easier to understand and modify in the future. By having the AI include comments as it generates code, you gain insight into the logic and structure behind the code, which can be particularly useful when revisiting the project later or when collaborating with others.

If the inline comments provided by the AI aren't sufficient or if certain parts of the code remain unclear, you can always ask the assistant for a more detailed explanation. This can help clarify complex sections of code, ensuring that you fully understand how the code operates and how it integrates into your broader project.

By consistently asking for comments and seeking additional explanations when needed, you enhance your comprehension of the codebase and make future development and maintenance tasks smoother and more efficient.

## Leverage AI for Diverse Coding Tasks

An AI assistant can be an invaluable tool across a wide range of coding activities, far beyond just generating new code. Consider using your AI assistant for the following tasks:

- Writing and Reviewing Database Scripts: AI can help you write complex SQL queries, create database schemas, and review existing scripts for errors or optimizations.
- Code Reviews and Pull Requests: Use AI to review pull requests, identify potential improvements, and ensure consistency across your codebase.
- Understanding Unfamiliar Code: If you encounter code that you didn’t write or aren’t familiar with, AI can help you understand its purpose and functionality by providing explanations or summaries.
- Creating New Functions and Utilities: AI can assist in writing new functions, whether they are utility functions or core components, ensuring that they are well-structured and meet your project’s needs.
- Discussing Software Patterns: You can consult the AI on the best software patterns to apply to specific problems, ensuring that your solutions are aligned with industry standards and best practices.
- Standardizing Modules: AI can help in the standardization of modules, ensuring that your codebase remains consistent and maintainable.
- Documenting Existing Code: Use AI to generate documentation for your existing code, including README files, API docs, and in-line comments.
- Writing and Reviewing Test Code: AI can assist in writing test cases or reviewing existing ones, ensuring that your code is thoroughly tested and reliable.

By leveraging the AI assistant for these diverse tasks, you can streamline your development process, reduce the time spent on routine activities, and ensure that your code is of high quality and well-documented.




