# Introduction

Organizations face unprecedented challenges, in the rapidly evolving digital landscape, such as increasingly sophisticated cyber threats and a significant talent shortage in cybersecurity. 

Microsoft Security Copilot is a cloud-based, AI-powered security analysis tool that is designed to address these challenges. 

It enables analysts to process security signals and respond to threats at a machine speed that far surpasses human capabilities, thus revolutionizing the way organizations approach cybersecurity.

---

**1. what Microsoft Security Copilot is?**

**2. Terminology of Microsoft Security Copilot?**

**3. how Microsoft Security Copilot processes prompt requests?**

**4. The elements of an effective prompt?**

**5. how to enable Microsoft Security Copilot?**

---

# Microsoft Security Copilot

The top security challenges organizations face include:

An increase in the number and sophistication of attacks.

A talent shortage that is driving the need for automation, integration, and consolidation of security tools.

Visibility into security, privacy, compliance, and governance.

Organizations need to act quickly to address all the security challenges they face, but working at human speed, even if there weren't a talent shortage, isn't enough. Organizations need to work at machine speed.

```

Microsoft Security Copilot is an AI-powered, cloud-based security analysis tool that enables analysts to respond to threats quickly

process signals at machine speed, and assess risk exposure more quickly than may otherwise be possible.
```

# Use cases

1. **Investigate and remediate security threats**
   
2. **Build KQL queries or analyze suspicious scripts**  -eliminate the need to manually write query-language scripts or reverse engineer malware scripts with natural language translation

3. **Understand risks and manage security posture of the organization**

4. **Troubleshoot IT issues faster**

5. **Define and manage security policies**

6. **Configure secure lifecycle workflows**

7. **Develop reports for stakeholders**

These use cases represent just a few of the capabilities that Copilot delivers and that helps make analysts more productive and also helps up-level them.

---

# Standalone and embedded experience

You can experience Copilot through the dedicated site, also referred to as the standalone experience. Users interact with Copilot through the prompt bar.

In the prompt bar, users make requests in natural language and receive response outputs as text, images, or documents.

<img width="1270" height="946" alt="image" src="https://github.com/user-attachments/assets/a0cd4704-8181-462f-8465-a21228b6dc5f" />

Additionally, some Microsoft security products embed Copilot capabilities directly within the products’ user interface. This experience is referred to as the embedded experience. Microsoft Defender XDR, for example, enables Copilot capabilities including summarizing incidents, analyzing scripts, generating KQL queries, and more.

Diagram that shows the advanced hunting page of Microsoft Defender XDR, The page includes a button for Copilot that When selected opens a side panel for natural language to KQL query assistant.

<img width="1510" height="936" alt="image" src="https://github.com/user-attachments/assets/f8cfc500-d484-42cd-bde5-38a29ff32d28" />

--- 
# Natural language processing (NLP)

Copilot is built using Azure OpenAI Services and is designed to integrate with existing security tools and processes, making it easier for organizations to improve their overall security posture. Azure OpenAI Services provides REST API access to OpenAI's powerful large language models (LLMs) for natural language processing (NLP), while providing security capabilities of Microsoft Azure.

# Integration with Security-specific sources

Copilot combines powerful LLMs with security-specific sources from Microsoft. These security-specific sources are informed by Microsoft’s unique global threat intelligence, more than 65 trillion daily signals, and incorporates information from a growing set of security solutions using plug-ins and connections to knowledge base

Through plug-ins, Copilot integrates with Microsoft's own security products, non-Microsoft products, and open-source intelligence feeds.

The information you give Copilot will only be accessible to your organization. Your data is your data, and it's protected by comprehensive enterprise compliance and security controls. Your data isn't used to train the foundation AI models.

<img width="690" height="635" alt="image" src="https://github.com/user-attachments/assets/29223a76-cfdc-4288-826a-e282f761db84" />

# Microsoft Security Copilot terminology

**Terminology**

The following terms are important for understanding the way Microsoft Security Copilot works:

**Session** – A particular conversation within Copilot. Copilot maintains context within a session.

**Prompt** – A specific statement or question within a session. A user enters a prompt in the prompt bar.

**Capability** – A function Copilot uses to solve part of a problem. A capability may sometimes be referred to as a skill.

**Plugin** – A collection of capabilities by a particular resource.

**Workspace** - Copilot workspaces are separate Copilot work environments within the tenant in which your Copilot instance is operating.

**Agents** - Microsoft Security Copilot agents are AI-powered tools that autonomously manage security and IT tasks.

**Orchestrator** – Copilot’s system for composing capabilities together to answer a user’s prompt.

# Prompt bar and sessions

At the center of Security Copilot is the prompt bar. You use the prompt bar to tell Copilot what insights you want from your security data, this is referred to as the prompt. In other words, the prompt is the text-based, natural language input you provide in the prompt bar that instructs Copilot to generate a response. 

<img width="650" height="78" alt="image" src="https://github.com/user-attachments/assets/9ecbc021-acbe-4d32-9d7f-8fe9f2527802" />


# Plugins and capabilities

In the previous unit, we mentioned that Copilot integrates with various sources through plugins, including Microsoft's own security products such as Microsoft Sentinel, Microsoft Defender XDR, and Microsoft Intune, non-Microsoft solutions, and open-source intelligence feeds. 

The integration enabled by the plugin, for any specific data source, provides Copilot with a collection of capabilities. Each capability is like a function in software, it’s designed to do a specialized task within the scope of the data source. 


For example, the plugin to Microsoft Defender XDR includes a collection of individual capabilities that are used only by Microsoft Defender XDR. These include:

The ability to summarize an incident.

Support incident response teams in resolving incidents through guided responses (a set of recommended actions based on the specific incident).

The ability to analyze scripts and code.

The ability to generate KQL queries from natural language input.

The ability to generate incident reports.


Copilot currently supports plug-ins for Microsoft services and non-Microsoft services, including websites and custom plug-ins that can be enabled.

<img width="526" height="524" alt="image" src="https://github.com/user-attachments/assets/caf486b3-9f7a-4c7d-917b-dfaea04316e1" />

<img width="526" height="653" alt="image" src="https://github.com/user-attachments/assets/fa8e27ae-0263-464d-a37a-357ec5be0cb1" />

# Workspaces

Copilot workspaces are separate Copilot work environments within the tenant in which your Copilot instance is operating.

To help you better understand the concept of workspaces, we'll use the analogy of house with multiple rooms. Each room is configured to be optimized for its function and the people that will use that room. When someone enters the house, they may have access to some rooms but not others.

<img width="1685" height="508" alt="image" src="https://github.com/user-attachments/assets/0c89a962-f096-47f0-9d64-54d77f925e5e" />

# Agents

A Microsoft Security Copilot agent is an advanced, AI-powered assistant built into Microsoft Security Copilot. These agents go beyond just answering questions—they can autonomously manage high-volume security and IT tasks. 

They’re deeply integrated with Microsoft’s security tools and can also work with partner solutions. Each agent is tailored for specific security scenarios, such as threat protection, identity management, or data security.

These agents are designed to learn from feedback, adapt to your organization’s workflows, and operate securely within Microsoft’s Zero Trust framework.

<img width="1385" height="750" alt="image" src="https://github.com/user-attachments/assets/c3b4f5a8-b1af-4eee-9b1f-1daff8927470" />

# how Microsoft Security Copilot processes prompt requests

**Process flow**

When a user submits a prompt, Copilot processes that prompt to generate the best possible response. The diagram that follows illustrates, at a high level, steps that Copilot takes to process the prompt and generate a response.

<img width="4036" height="1457" alt="image" src="https://github.com/user-attachments/assets/5a86e2a4-9707-4f59-8ead-eec2ed23ba39" />

