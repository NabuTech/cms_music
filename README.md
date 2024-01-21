# cms_music

# Project Structure

- **codeception/**          # Codeception configuration and tests
  - **acceptance/**        # Acceptance tests
  - **functional/**        # Functional tests
  - **unit/**              # Unit tests
  - **_bootstrap.php**     # Codeception bootstrap file
  - **codeception.yml**    # Codeception configuration file

- **public/**               # Webroot directory (CMS and web-related files)
  - **index.php**          # Main entry point for the website
  - **assets/**            # CSS, JS, images, etc.

- **src/**                  # PHP source code
  - **Controller/**        # Controllers for your CMS
  - **Model/**             # Models or data structures
  - **View/**              # Views or templates

- **tests/**                # Additional tests (outside Codeception)

- **vendor/**               # Composer dependencies

- **.gitignore**            # Git ignore file
- **composer.json**         # Composer configuration
- **composer.lock**         # Composer lock file

# Workflow

1. Codeception Tests                      Learn Codeception and Run Tests
2. CMS Integration                        Controllers for Different Pages
3. Webroot and Assets                     Place web files in public directory
4. Composer Dependencies                  Manage Php dependencies using Composer.Run
5. Keep Project Documentation up to date  Project Structure, CMS Configurations
6. Review and Refactor                    Regular review and refactor code as needed
