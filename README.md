# 🚀 My n8n Project (n8n-projects)

Welcome to my n8n project repository!  
This is a collection of workflows and custom nodes I use to automate various tasks.

## 📁 Repository Structure

- **/workflows**: Contains all `.json` n8n workflow files. You can import them directly into your n8n instance.  
- **/nodes**: *(Optional)* Contains code for [custom n8n nodes](https://docs.n8n.io/create-nodes/introduction/) that I’ve created.

## ⚙️ How to Use the Workflows

Each workflow in the `/workflows` folder is an independent JSON file.

1. **Download** the `.json` file you need.  
2. **Import into n8n:**  
   - Open your n8n canvas.  
   - Use the shortcut `Ctrl + I` (or `Cmd + I` on Mac) to **Import from File**.  
   - Select the `.json` file you downloaded.

## ⚠️ Credential Warning

**This repository does not store any credentials (API keys, tokens, or passwords).**  

When you import a workflow, you must configure your own **Credentials** inside your n8n instance for it to work properly.

---

💡 *Tip:* Always review each workflow before running it to understand what it does and ensure it meets your security requirements.
