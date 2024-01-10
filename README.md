

```markdown
# internsctl

## Description

`internsctl` is a custom Linux command-line tool designed to manage interns and perform various system-related tasks. This repository contains the script and associated files for `internsctl`.

## Features

- List all interns.
- Add and remove interns.
- Obtain CPU and memory information.
- Manage users: create, list regular users, and list users with sudo permissions.
- Retrieve information about files.

## Usage

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/internsctl.git
   ```

2. Move into the project directory:

   ```bash
   cd internsctl
   ```

3. Make the script executable:

   ```bash
   chmod +x internsctl
   ```

4. Copy the manual page to the appropriate directory:

   ```bash
   sudo cp internsctl.1 /usr/share/man/man1/
   ```

   **Note:** Replace `internsctl.1` with your actual manual page file name.

5. Update the manual page database:

   ```bash
   sudo mandb
   ```

### Commands

- List all interns:

  ```bash
  ./internsctl list
  ```

- Add an intern:

  ```bash
  ./internsctl add JohnDoe
  ```

- Remove an intern:

  ```bash
  ./internsctl remove JaneSmith
  ```

- Get CPU information:

  ```bash
  ./internsctl cpu getinfo
  ```

- Get memory information:

  ```bash
  ./internsctl memory getinfo
  ```

- Create a new user:

  ```bash
  ./internsctl user create username
  ```

- List all regular users:

  ```bash
  ./internsctl user list
  ```

- List users with sudo permissions:

  ```bash
  ./internsctl user list --sudo-only
  ```

- Get information about a file:

  ```bash
  ./internsctl file getinfo filename
  ```

  - Options for specific information:

    ```bash
    ./internsctl file getinfo --size filename
    ./internsctl file getinfo --permissions filename
    ./internsctl file getinfo --owner filename
    ./internsctl file getinfo --last-modified filename
    ```

### Documentation

For full documentation and usage details, refer to the manual page:

```bash
man internsctl
```

## Contributing

Feel free to contribute to this project by opening issues or pull requests. Your feedback and contributions are highly appreciated.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

Replace the placeholder values such as `your-username` and customize the content to fit the specifics of your project. Additionally, ensure that the actual file names match those in your project directory.
