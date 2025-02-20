# My Personal Blog

- [About](#about)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## About

This blog is built using Jekyll and the Minimal Mistakes theme. It includes posts on various topics such as software engineering, personal growth, and life in Japan.

Jekyll is a static site generator written in Ruby. It takes your content, such as Markdown files, and a set of templates, and produces a complete, static website ready to be served by a web server. Here are some advantages of using Jekyll over a more robust platform like WordPress:

1. Performance: Since Jekyll generates static HTML files, the resulting website is typically faster than a dynamic site like WordPress, which relies on a database and server-side processing for each page request.

2. Security: Static sites have a smaller attack surface compared to dynamic sites. There are no databases, server-side scripts, or plugins that can be exploited.

3. Simplicity: Jekyll sites are simple to set up and maintain. There are no databases to manage, and the content is written in Markdown, which is easy to learn and use.

4. Version Control: Jekyll sites can be version-controlled using Git, making it easy to track changes, collaborate with others, and roll back to previous versions if needed.

5. Customization: Jekyll offers a high degree of customization through its templating system. You can create custom layouts and include reusable components.

6. Hosting: Jekyll sites can be hosted on GitHub Pages for free, which is a convenient and cost-effective option for many users.

7. No Dependencies: Unlike WordPress, which requires a PHP environment and a MySQL database, Jekyll only requires Ruby and a few gems, making it easier to set up and deploy.

Overall, Jekyll is a great choice for developers who prefer a lightweight, secure, and fast solution for their websites, especially for blogs and documentation sites.

## Installation

To set up the blog locally, follow these steps:

1. Clone the repository:

    ```sh
    git clone https://github.com/reecewithnospoon/reecewithnospoon.github.io.git
    cd reecewithnospoon.github.io
    ```

2. Install the required gems:

    ```sh
    bundle install
    ```

3. Serve the site locally:

    ```sh
    bundle exec jekyll serve
    ```

4. Open your browser and navigate to `http://localhost:4000`.

## Usage

### Adding a New Post

1. Create a new file in the  directory with the following naming convention: `YYYY-MM-DD-title.md`.
2. Add the front matter to the top of the file:

    ```md
    ---
    title: "Your Post Title"
    date: YYYY-MM-DD HH:MM:SS +/-TTTT
    categories: [category1, category2]
    header:
      overlay_image: "/assets/images/your-image.jpg"
    ---
    ```

3. Write your content below the front matter.

### Customizing the Navigation

Edit the  file to update the navigation links.

### Changing the Site Configuration

Edit the  file to update the site settings such as title, description, and social links.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.