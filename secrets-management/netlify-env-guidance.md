# Netlify Environment Guidance

Netlify environment variables should be configured in Netlify rather than committed to GitHub. Build settings must match the framework. Deploy previews should be reviewed before production deploys or client handoff.

## Checklist
1. Confirm framework.
2. Confirm build command.
3. Confirm publish directory.
4. Confirm required environment variables.
5. Add env vars in Netlify.
6. Trigger deploy preview.
7. Review build logs.
8. Test live URL.
9. Approve production deploy.
10. Document handoff notes.
