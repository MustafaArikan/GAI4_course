# GAI4 Course

## Setup

### 1. Clone the repository

```bash
git clone --recurse-submodules https://github.com/MustafaArikan/GAI4_course.git
cd GAI4_course
```

If you already cloned without `--recurse-submodules`:

```bash
git submodule update --init --recursive
```

### 2. Install dependencies

Install [uv](https://docs.astral.sh/uv/getting-started/installation/) if you don't have it:

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Then set up the environment for the unit you want to work on:

```bash
cd Unit_0
uv sync
```
