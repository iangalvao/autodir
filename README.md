# Project Tree Generator

A Python script that creates a project directory and file structure from a tree-like representation provided in a text file. This is useful for quickly initializing project scaffolding for development.

## Features

- Parses a tree-like structure from a text file.
- Supports arbitrary levels of nesting for directories and files.
- Creates both empty directories and files based on the given structure.

## Requirements

- Python 3.6+

## Installation

Clone the repository:

   ```bash
   git clone https://github.com/iangalvao/autodir.git
   cd autodir
   ```

## Usage

1. Create a text file containing your desired project structure. For example:

   ```
   task-manager/
   ├── backend/
   │   ├── Dockerfile
   │   ├── requirements.txt
   │   ├── manage.py
   │   ├── task_manager/
   │   └── tasks/
   ├── frontend/
   │   ├── Dockerfile
   │   ├── package.json
   │   ├── src/
   │   └── public/
   └── docker-compose.yml
   ```

2. Run the script:

   ```bash
   python project_tree_init.py <path_to_tree_file> <output_directory>
   ```

   - `<path_to_tree_file>`: Path to the text file containing the tree structure.
   - `<output_directory>`: Path to the directory where the project structure will be created. Use ./ to create in the working directory

3. Example:

   ```bash
   python project_tree_init.py example_tree.txt ./my_project
   ```

   This will create the project structure under `./my_project`.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request with your improvements or bug fixes.

## Author

[Ian Galvão](https://github.com/iangalvao)

