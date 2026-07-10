# Statistics Textbooks Question Bank

This repository contains the Moodle question bank for the **Statistics Textbooks** project. Questions are authored in Moodle using STACK and synchronised with Git using the Moodle **qbank_gitsync** plugin.

The repository is intended to provide version control, collaboration, and a portable archive of the question bank.

## Repository structure

```
statistics-textbooks/
├── question-datasets/
├── top/
│   ├── Category 1/
│   ├── Category 2/
│   └── ...
└── ecampus_course_..._manifest.json (local only, ignored by Git)
```

- `top/` contains the exported question bank organised according to the Moodle question category structure.
- Each question is stored as an individual Moodle XML file.
- `gitsync_category.xml` files describe the category hierarchy and are maintained automatically by Gitsync.
- The Gitsync manifest is **not committed** because it contains Moodle instance-specific information.

## Datasets

The `question-datasets/` directory contains datasets used by questions in this repository.

These files are version controlled alongside the questions so that:

- each revision of a question references the correct version of its dataset;
- contributors can reproduce questions without relying on external storage;
- datasets remain available when the repository is cloned or archived.

Questions should reference the raw GitHub URLs for these datasets when offering them for download.

## Workflow

### Editing questions in Moodle

1. Edit and save the question in Moodle.
2. Export the changes:

   ```bash
   php exportrepofrommoodle.php
   ```

3. Review the Git diff.
4. Commit the changes.
5. Push to GitHub.

### Editing questions in Git

1. Modify the XML files.
2. Review the Git diff.
3. Commit the changes.
4. Import into Moodle:

   ```bash
   php importrepotomoodle.php
   ```

5. Verify the imported question in Moodle.
6. Push to GitHub.

> **Note:** `importrepotomoodle.php` requires a clean Git working tree before importing.

## Requirements

This repository assumes:

- Moodle with the `qbank_gitsync` plugin installed.
- A configured `config.php` in the local Gitsync CLI directory.
- Git.
- PHP with the required extensions enabled (including `curl` and `openssl`).

## Files not committed

The following files are intentionally excluded from version control:

- Gitsync manifest (`*_question_manifest.json`)
- Temporary files (`*.tmp`)
- Editor-specific configuration (e.g. `.vscode/`)

## Contributing

Before submitting changes:

- review the Git diff;
- ensure questions behave correctly in Moodle;
- keep datasets in `question-datasets/`;
- use meaningful commit messages describing the educational change.