Here’s the complete guide to the Prompt-Query-Exchange (PQE) format rewritten in GitHub-flavored Markdown:

# Prompt-Query-Exchange (PQE) Format Guide

## Introduction
The **Prompt-Query-Exchange (PQE)** format is designed to document interactions with AI language models. This structured approach helps researchers and developers track prompt engineering sessions, assess AI responses, and facilitate iterative improvement in AI interactions.

## Structure of the PQE Format

The PQE format consists of several key sections:

### 1. Meta Section
This section captures overarching information about the session.

```json
{
  "meta": {
    "title": "Title of the Session",
    "researcher": "Your Name",
    "date": "YYYY-MM-DD",
    "tool": "AI Tool Used (e.g., ChatGPT)",
    "version": "Model Version",
    "objective": "Goal of the Interaction",
    "context": "Relevant Environmental Details"
  }
}
```

2. Interactions Section

This section contains an array of each prompt-response pair.

```
"interactions": [
  {
    "id": 1,
    "prompt": {
      "text": "Your prompt text here",
      "intent": "Purpose of the prompt (e.g., initial inquiry)",
      "tags": ["relevant", "keywords", "related"]
    },
    "response": {
      "text": "AI response text here",
      "rating": "Assessment of the response (e.g., complete, partial)",
      "issues": ["Any issues encountered with the response"]
    }
  }
]
```

3. Summary Section

This section provides an overview of the session’s outcomes.

```
"summary": {
  "iterations": Total number of interactions,
  "final_prompt": "Final refined prompt used",
  "final_output": "Final usable result from the session",
  "lessons_learned": "Key takeaways from the interaction"
}
```

4. Attachments Section

This section includes any relevant supporting materials.

```
"attachments": {
  "code": "Relevant code snippets or examples",
  "logs": "Links to complete chat logs or related documentation"
}
```

Example PQE Document

Here’s an example of a complete PQE document:
```
{
  "meta": {
    "title": "Tracking Hexbug with OpenCV",
    "researcher": "Dr. Trevor M. Tomesh",
    "date": "2024-10-16",
    "tool": "ChatGPT (GPT-4)",
    "version": "4.0",
    "objective": "To develop a method for tracking a hexbug using OpenCV",
    "context": "Using Python and OpenCV for image processing"
  },
  "interactions": [
    {
      "id": 1,
      "prompt": {
        "text": "How can I track a hexbug in OpenCV using template matching?",
        "intent": "initial inquiry",
        "tags": ["OpenCV", "template matching", "tracking"]
      },
      "response": {
        "text": "You can use OpenCV’s cv2.matchTemplate function for template matching. Here’s an example...",
        "rating": "complete",
        "issues": []
      }
    }
  ],
  "summary": {
    "iterations": 1,
    "final_prompt": "How can I track a hexbug in OpenCV using template matching?",
    "final_output": "Code example for hexbug tracking.",
    "lessons_learned": "Effective tracking can be achieved using template matching."
  },
  "attachments": {
    "code": "Python code snippet here...",
    "logs": "Link to relevant documentation"
  }
}
```
Prompt Instructions for Generating a PQE Report

When tagging onto the end of a conversation to generate a PQE report, use the following instructions:

```
Now, please create a detailed Prompt-Query-Exchange (PQE) report based on this conversation. The output should be in a JSON-like format, structured as follows:

{
  "meta": {
    "title": "Title of the Session",
    "researcher": "Your Name",
    "date": "YYYY-MM-DD",
    "tool": "AI Tool Used (e.g., ChatGPT)",
    "version": "Model Version",
    "objective": "Goal of the Interaction",
    "context": "Relevant Environmental Details"
  },
  "interactions": [
    {
      "id": 1,
      "prompt": {
        "text": "Your prompt text here",
        "intent": "Purpose of the prompt (e.g., initial inquiry)",
        "tags": ["relevant", "keywords", "related"]
      },
      "response": {
        "text": "AI response text here",
        "rating": "Assessment of the response (e.g., complete, partial)",
        "issues": ["Any issues encountered with the response"]
      }
    }
  ],
  "summary": {
    "iterations": Total number of interactions,
    "final_prompt": "Final refined prompt used",
    "final_output": "Final usable result from the session",
    "lessons_learned": "Key takeaways from the interaction"
  },
  "attachments": {
    "code": "Relevant code snippets or examples",
    "logs": "Links to complete chat logs or related documentation"
  }
}

Make sure to fill in the relevant details in each section, including the meta section with the title, researcher name, date, tool, and context. For the interactions section, number each interaction and include the prompt, response, rating, and any issues. In the summary section, provide an overview of the total iterations, final prompt, final output, and lessons learned. Finally, include any relevant code or links in the attachments section.
```

### Conclusion

The PQE format provides a systematic way to document and analyze interactions with AI models, promoting better understanding and improvement of AI applications.

Credits

This guide was created by ChatGPT in collaboration with Dr. Trevor M. Tomesh, University of Wisconsin - River Falls, Department of Computer Information and Data Science.
