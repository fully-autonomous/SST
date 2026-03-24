# Documentation Updates Summary

## Issues Resolved

### 1. #2060: Add server instructions documentation to main docs

**Status**: ✅ **RESOLVED**

**What was done**:
- Copied and adapted content from the blog post "Server Instructions: Giving LLMs a user manual for your server" (https://blog.modelcontextprotocol.io/posts/2025-11-03-using-server-instructions/)
- Added comprehensive guidance on server instructions to the main documentation
- Included best practices, implementation tips, and examples

**Where**: `docs/docs/learn/server-concepts.mdx`

**Key additions**:
- Detailed explanation of what server instructions are and why they matter
- Anti-patterns to avoid when writing instructions
- Implementation guidance for both server developers and client implementers
- Progressive disclosure concepts for better LLM integration

### 2. #2064: Add guidance on session affinity for Mcp-Session-Id in stateful deployments

**Status**: ✅ **RESOLVED**

**What was done**:
- Added a new "Session Affinity for Stateful Deployments" section
- Included guidance on using session affinity for stateful deployments
- Added practical recommendations for multi-worker load balancing
- Provided context on operational implications of session management

**Where**: `docs/docs/learn/server-concepts.mdx`

**Key additions**:
- Explanation of session affinity requirements
- Guidance on externalized session state
- Recommendations for distributed caching
- Monitoring suggestions for session-related failures

### 3. #2146: Provide guidance on how to set/use server description/instructions

**Status**: ✅ **RESOLVED**

**What was done**:
- Expanded the server description/instructions section with comprehensive guidance
- Added clear distinction between description and instructions purposes
- Included progressive disclosure concepts
- Added implementation tips and best practices

**Where**: `docs/docs/learn/server-concepts.mdx`

**Key additions**:
- Purpose and audience clarification for both fields
- Key differences between description and instructions
- Implementation tips for setting both fields
- Model-agnostic writing guidance

## Summary

All three documentation gaps have been resolved with comprehensive, practical guidance that will help both server developers and client implementers better understand and implement MCP server features. The documentation now provides clear guidance on:

1. Server instructions - how to write them, when to use them, and best practices
2. Session affinity - operational guidance for stateful deployments
3. Server description/instructions - how to set them and their key differences

The changes maintain consistency with existing documentation style while adding substantial new content to address the identified gaps.

## Verification

- All documentation checks pass (`npm run check` and `npm run prep`)
- Changes committed to main branch
- Working tree is clean
- No broken links or formatting issues