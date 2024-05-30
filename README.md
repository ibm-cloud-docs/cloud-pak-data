# cloud-pak-data

Documentation repository for "Cloud Pak for Data" at <staging>[pre-production output](https://test.cloud.ibm.com/docs/cloud-pak-data).</staging><publish>[production output](https://cloud.ibm.com/docs/cloud-pak-data).

:information_source: **Tip:** If you want to give feedback about the documentation, create an [issue](https://github.ibm.com/cloud-docs/cloud-pak-data/issues).

</publish>

<staging>

## Creating content

Follow these steps to add to the Cloud Pak for Data on IBM Cloud docs.

:information_source: **Tip:** If you'd rather give feedback about the documentation, create an [issue](https://github.ibm.com/cloud-docs/cloud-pak-data/issues).

### Before you begin
Set up your local development environment

- Visual Studio Code is the recommended editor. For more information, see [Choose an editor](https://test.cloud.ibm.com/docs-internal/writing?topic=writing-setting-up-your-markdown-environment#choose-an-editor).
- You can install a Markdown linter in Visual Studio Code that works with IBM Cloud docs. For more information, see [Integrating the Markdown linter in VS Code](https://test.cloud.ibm.com/docs-internal/writing?topic=writing-markdown-linter-vscode).

### Drafting content

All content starts from the `source` branch.

1.  Clone this repo if you have write privileges. Otherwise, fork the repo.
1.  Create a working branch from the `source` branch.
1.  Make your changes to the Markdown content.

    - Cloud docs uses Markdown with a few custom extensions to source the docs. For tips about how to structure and style your docs with IBM Cloud Markdown, see [Quick tips for authoring in IBM Cloud docs](https://test.cloud.ibm.com/docs-internal/writing?topic=writing-solution-guides#solution-guides-include-quick-tips) in "Creating solution, deployment, and migration guides".
    - Cloud docs also supports controlling content with tagging. For example, content within the <code>&lt;staging&gt;</code>&nbsp;<code>&lt;/staging&gt;</code> tags is not displayed to the public. For more information, see [Making updates to your docs](https://test.cloud.ibm.com/docs-internal/writing?topic=writing-update-docs).

1.  Commit your updates.
1.  Create a pull request from your branch or fork to `source`.

    1.  A Jenkins job runs that commits content to the `draft` and `review` branches and opens a pull request to the `publish` branch.
    1.  After a few minutes, you can see your changes in the IBM Cloud docs framework. Changes to `draft` are available at the internal `/docs-draft/` location (https://test.cloud.ibm.com/docs-draft/cloud-pak-data?topic=cloud-pak-data-getting-started). Changes to `review` are available at the pre-production `/docs/` location (https://test.cloud.ibm.com/docs/cloud-pak-data?topic=cloud-pak-data-getting-started).

:information_source: **Tip:** Content that is tagged with <code>&lt;draft&gt;</code>, <code>&lt;review&gt;</code>, <code>&lt;staging&gt;</code>, or feature tags are built and promoted only to the internal location and is not included in the pull request to the `publish` branch for production.
</staging>
