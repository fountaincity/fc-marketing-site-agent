# Fountain City AI Chat Widget Documentation

## Overview
The Fountain City AI Chat Widget implements a hierarchical conversation flow designed to guide users through different types of interactions. The system uses Claude 3.5 Sonnet as its underlying language model and is structured to handle various user intents while maintaining brand consistency.

## Workflow Hierarchy
1. **Start (Home)** - Initial entry point
2. **Book a Demo** - Sales and consultation requests
3. **Submit a Ticket** - Technical support issues
4. **Knowledge Base Response** - Catch-all for general inquiries

## Workflow Details
Spreadsheet has triggers, messages, and prompts for Book a Demo and Submit a Ticket

### 1. Start (Home)
- Primary entry point for all conversations
- Handles initial user greetings and directs to appropriate workflow
- Routes users based on detected intent

### 2. Book a Demo
- **Purpose**: Handle sales inquiries and consultation requests
- **Trigger Conditions**: 
  - Explicit requests for demos
  - Consultation requests
  - Project discussion requests
  - Pricing inquiries
- **Response**: "Click through to our discovery form to set your project in motion."
- **Important Note**: Pricing inquiries are directed to the contact form rather than providing specific pricing information

### 3. Submit a Ticket
- **Purpose**: Handle technical support requests and issue reporting
- **Trigger Conditions**:
  - Technical assistance requests
  - Bug reports
  - Website issues
  - Support ticket creation
- **Response**: "Let's get you over to our contact form so our team can review your issue."

### 4. Knowledge Base Response
- **Purpose**: Catch-all for general inquiries
- **Handles**:
  - General questions about services
  - Information requests
  - Any queries not matching other workflows

## Implementation Guidelines

### Intent Recognition
- System prioritizes explicit demo/sales requests over general inquiries
- Technical support issues are routed to ticket submission
- General questions default to knowledge base responses

### Response Handling
1. **Sales Inquiries**:
   - Direct to discovery form
   - Avoid providing specific pricing
   - Focus on understanding client needs

2. **Technical Support**:
   - Prompt ticket creation
   - Direct to Contact Form

3. **General Inquiries**:
   - Provide knowledge base information
   - Maintain brand voice
   - Escalate to appropriate workflow if needed

## Best Practices

1. **Maintain Brand Voice**
   - Clear and professional tone
   - Focus on process and methodology
   - Emphasize validation-first approach

2. **User Experience**
   - Clear pathways to resolution
   - Consistent messaging
   - Appropriate escalation paths

3. **Response Priority**
   - Sales inquiries take precedence
   - Technical issues route to support
   - General queries default to knowledge base

## Maintenance and Updates

- Regular review of trigger phrases
- Update knowledge base responses
- Monitor conversation flows
- Adjust routing logic as needed


QA Sheet
[qasheet](https://docs.google.com/spreadsheets/d/1TjwhutOcgE3cg2MTvNA0s_uFyRNB6a5H8xYmjbvfCic/edit?gid=0#gid=0)
