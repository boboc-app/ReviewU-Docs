# ReviewU
- [ReviewU Example](https://github.com/boboc-app/ReviewU-examples)

## Introduction
ReviewU is a GitHub App designed to streamline your code review process by automatically summarizing Pull Request changes. By providing clear and concise PR summaries, ReviewU helps developers quickly understand key modifications without sifting through extensive diff logs.

## Guide

### Main Configuration
The primary configuration for ReviewU is managed within the `.review_u` directory. All files in this directory are excluded from the PR summary generation. Once installed, ReviewU is immediately active, and these configuration settings are optional.

### [Optional] Configuration Settings
To customize ReviewU's behavior, create a configuration file named `.reviewuConfig` inside the `.review_u` directory. This YAML file allows you to tailor which files to ignore, specify PR title patterns that should skip summary generation, and set the language for your summaries:

```yaml
# .review_u/.reviewuConfig
excludes:  # List of files or directories to exclude from PR summary analysis
  - build.gradle.kts
  - .env*
  - **/test/**
exclude-titles:  # PR title patterns that will not trigger a summary
  - Release/**
  - Minor/**
language-code: EN  # Language for PR summaries (e.g., EN, KR, JP, CN). Default is EN.
```

### [Optional] Format Customization
If you wish to customize the format of the generated PR summaries, create a file named `SUMMARIZER_FORMAT.md` in the `.review_u` directory. This file lets you define separate sections for major and minor changes, ensuring that the summary fits your team’s style:

```markdown
# .review_u/SUMMARIZER_FORMAT.md

## Major Changes
<!-- Summarize core modifications that impact business logic or primary functionality.
Example:
1. Modify 'AA' function logic  
   - Updated algorithm from 'OO' to 'XX'.
2. Add 'OOO' Classes  
   - Introduced 'OOO' class to handle 'XXX' functionality.
-->

## Minor Changes
<!-- Summarize non-critical modifications such as updates to build configurations, documentation, or assets. -->
```

### Limitations
ReviewU adheres to GitHub’s inherent repository constraints, including:
- [Repository Limits](https://docs.github.com/en/repositories/creating-and-managing-repositories/repository-limits)
- [Diff Limits](https://docs.github.com/en/repositories/creating-and-managing-repositories/repository-limits#diff-limits)
- [Commit Listings Limits](https://docs.github.com/en/repositories/creating-and-managing-repositories/repository-limits#commit-listings-limits)

These limitations might affect the summarization of extremely large or complex pull requests.

## FAQ
**Q: Do I need to set up configurations immediately after installation?**  
A: No. ReviewU works out-of-the-box. The configuration settings are optional and can be customized later.

**Q: How do I change the language for PR summaries?**  
A: Update the `language-code` field in the `.reviewuConfig` file with your desired language code (e.g., EN, KR).

**Q: Can I exclude certain files or directories from being summarized?**  
A: Yes. Use the `excludes` field in the `.reviewuConfig` file to list files or directories that should be ignored during summary generation.

## Conclusion
ReviewU is crafted to enhance your code review workflow by automatically generating concise and focused PR summaries. Customize the configuration and format to align with your team’s needs, and enjoy a more efficient and productive review process!

<hr/>
<br/>
<br/>
@ Contact: `bo.kang@boboc.app`
