# cms_music

## Project Structure

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

## Workflow

1. Codeception Tests                      Learn Codeception and Run Tests
2. CMS Integration                        Controllers for Different Pages
3. Webroot and Assets                     Place web files in public directory
4. Composer Dependencies                  Manage Php dependencies using Composer.Run
5. Keep Project Documentation up to date  Project Structure, CMS Configurations
6. Review and Refactor                    Regular review and refactor code as needed

## Database Structure

For a simple CMS application tailored to a musician's personal site, you might need a database structure that allows you to store content for different pages. Here's a basic first draft for the database structure using MySQL:

### Tables:

1. **Pages:**
   - `page_id` (Primary Key)
   - `title` (Title of the page, e.g., Homepage, About Me, Pricing, Testimonials, Contact)
   - `content` (Text content of the page, possibly long text)
   - `created_at` (Timestamp for when the page was created)
   - `updated_at` (Timestamp for when the page was last updated)

### SQL Script:

```sql
CREATE TABLE pages (
    page_id INT PRIMARY KEY AUTO_INCREMENT,
    title VARCHAR(255) NOT NULL,
    content TEXT,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP
);
