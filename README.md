# Manual segmentation template

This is a template for a manual segmentation project. It contains the code for the pre-processing of the point clouds and the quality check at the end.

It ensures a standard format is used across all projects.

## Requirements

You need to install two tools before you can use this template. You only need to do this once.

### 1. Install pixi

pixi manages all the software dependencies for you automatically.

1. Go to [https://pixi.sh/](https://pixi.sh/)
2. Follow the installation instructions for your operating system
3. To check it worked, open a terminal and type `pixi --version` — you should see a version number

### 2. Install copier

copier creates a new project folder from this template.

1. Open a terminal
2. Copy and paste this command, then press Enter:
   ```
   pixi global install copier
   ```
3. To check it worked, type `copier --version` — you should see a version number

## Usage

### Create a new project

1. Open a terminal in the folder where you want to create your project
2. Run:
   ```
   copier copy https://github.com/mone27/manual-seg-template .
   ```
3. You will be asked for your **project name** — type it and press Enter (e.g. `Mount_fisher`)
4. Your new project folder is ready!

### Apply the template to an existing project

If you already have a project folder, you can apply the template to it directly:

```
copier copy https://github.com/mone27/manual-seg-template path/to/your-project
```

Copier will ask you what to do if any files already exist (keep yours or overwrite). You can also run `copier update` later to pick up any future changes to the template.

### Set up the project environment

Once inside your project folder, run:
```
pixi install
```
This will automatically download and install all required software. It may take a few minutes the first time.

### Run the quality check

Open the `processing/quality_check.ipynb` notebook and run the cells from top to bottom either in VS Code or Jupyter Lab.

## Optional features

### Pretty names (`processing/pretty/`)

The `processing/pretty/` subfolder contains notebooks for working with pretty names during segmentation (e.g. "Lama_04" instead of "FIS01-02_345970_8059550_04")
This is optional as it a matter of personal preference

When creating a project with copier, you will be asked to include the pretty names feature.

Answer `y` to include it, or just press Enter to skip it.


# Status

the pre-processing code will be added soon