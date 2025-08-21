# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a research repository containing reverse engineering analysis of Claude Code v1.0.33. The repository focuses on understanding the architecture, mechanisms, and implementation patterns of modern AI Agent systems through systematic analysis of obfuscated source code.

## Project Structure

### Main Analysis Workspace
- `claude_code_v_1.0.33/stage1_analysis_workspace/` - Complete analysis results for v1.0.33
- `chunks/` - Deobfuscated code chunks (102 files) split from the main CLI file
- `docs/` - Comprehensive technical documentation and analysis reports
- `scripts/` - Analysis tools and utilities for processing obfuscated code

### Key Directories
- `analysis_results/merged-chunks/` - Optimized and merged code blocks
- `docs/Open-Claude-Code/` - Open source reconstruction project template
- `work_doc_for_this/` - Project methodology and standard operating procedures

## Common Commands

Based on the analysis workspace structure, the following commands are commonly used:

### Code Analysis and Processing
```bash
# Beautify and format obfuscated code
node scripts/beautify.js source/cli.mjs

# Split large files into manageable chunks
node scripts/split.js cli.beautify.mjs

# Merge and improve code chunks
node scripts/merge-again.js

# LLM-assisted analysis of code segments
node scripts/llm.js
```

### Development Commands (Open-Claude-Code Project)
```bash
# Build TypeScript project
npm run build

# Run tests with coverage
npm run test:coverage

# Performance benchmarking
npm run benchmark

# Code quality checks
npm run lint
npm run validate

# Development mode
npm run dev
```

## Architecture Insights

### Core Technical Discoveries

1. **h2A Async Message Queue System** - Real-time steering mechanism with dual-buffer architecture
2. **Multi-layered Agent Architecture** - Main agent loop (nO), sub-agents (I2A), and task-specific agents
3. **Intelligent Context Management** - 92% threshold auto-compression with wU2 compressor
4. **6-Layer Security Framework** - From UI validation to execution sandboxing

### Key Components Analyzed

- **Agent Loop System** - Asynchronous generator-based core scheduler
- **Tool Execution Framework** - 6-stage pipeline with concurrency control
- **Memory Management** - Dynamic context compression and token optimization
- **Security Framework** - Multi-layer permission validation and sandboxing

## Analysis Methodology

### Static Code Analysis
1. **Code Preprocessing** - Deobfuscation and formatting
2. **Intelligent Chunking** - Breaking large files into analyzable segments
3. **LLM-Assisted Pattern Recognition** - Using AI to identify architectural patterns
4. **Cross-Validation** - Multiple rounds of verification for accuracy

### Documentation Standards
- All technical assertions must have source code location references
- Cross-document consistency validation required
- Minimum 95% accuracy threshold for final reports
- Complete lifecycle coverage from UI to execution

## Research Focus Areas

1. **Real-time Message Processing** - h2A dual-buffer mechanisms
2. **Agent Orchestration** - Multi-agent coordination patterns  
3. **Context Management** - Intelligent compression and memory optimization
4. **Security Architecture** - Layered protection and sandboxing
5. **Tool Integration** - Plugin-based execution framework

## Important Files

- `Claude_Code_Agent系统完整技术解析.md` - Complete technical analysis
- `FINAL_VALIDATION_REPORT.md` - Comprehensive validation results
- `实时Steering机制完整技术文档.md` - Real-time steering mechanism details
- `分层多Agent架构完整技术文档.md` - Multi-agent architecture analysis

## Development Guidelines

When working with this repository:

1. **Analysis Work** - Follow the established SOP in `work_doc_for_this/`
2. **Code Quality** - Maintain high standards for any new analysis scripts
3. **Documentation** - All findings must be properly documented with source references
4. **Validation** - Cross-verify technical claims across multiple documents
5. **Research Ethics** - This is for educational and research purposes only

## Notes

- This repository contains research analysis, not production code
- The analysis is based on obfuscated source code with inherent limitations
- All findings should be considered approximations for educational purposes
- The Open-Claude-Code project provides TypeScript implementations based on analysis