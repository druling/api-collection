# Druling API Collection

A comprehensive API collection for the Druling platform, organized into modular services with environment configurations.

## Setup

We use bruno for our API Client. https://www.usebruno.com/ you can download bruno as a app or plugin in you VScode.

## Overview

This repository contains API definitions for three main services:
- **AI Server** - AI-powered conversation and asset processing endpoints
- **Backend** - Core application services including auth, workflows, and file management
- **MCP Server** - Model Context Protocol tools and services

## Structure

```
api-collection/
├── collections/          
│   ├── ai-server/       
│   ├── backend/         
│   └── mcp-server/       environments/            
│   ├── Beta.yml
│   ├── Dev Druling.yml
│   ├── Local copy.yml
│   └── Production.yml
└── workspace.yml        
```

## Environments

Four preconfigured environments are available:

| Environment | Description |
|------------|-------------|
| **Local** | Local development setup |
| **Dev Druling** | Development server |
| **Beta** | Beta testing environment |
| **Production** | Production server |

Each environment contains specific configuration for:
- Base URLs
- API keys
- Authentication tokens
- Service endpoints

## Usage

1. **Select an Environment**: Choose the appropriate environment (Local, Dev, Beta, or Production)
2. **Navigate to Collection**: Browse to the desired service collection
3. **Execute Requests**: Run API requests using the configured endpoints
4. **Health Checks**: Each service includes a Health Check endpoint for monitoring

## Health Check Endpoints

All services include health check endpoints for system monitoring:
- `ai-server/Health Check.yml`
- `backend/Health Check.yml`
- `mcp-server/health.yml`
