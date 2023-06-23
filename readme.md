# Bookmark Manager

This is a simple bookmark manager application built with HTML, CSS, and JavaScript. It allows users to save and manage bookmarks for their favorite websites.

## Features

- **Add Bookmark:** Users can add a new bookmark by providing the name and URL of the website.
- **Validation:** The form validates that both the name and URL fields are filled. It also checks if the URL is in a valid format.
- **Delete Bookmark:** Each bookmark has a delete button that allows users to remove it from their bookmarks list.
- **Persistent Storage:** The bookmarks are stored in the browser's local storage, so they are preserved even after closing the application.

## Usage

To use the bookmark manager, follow these steps:

1. Open the application in a web browser.
2. Click on the "Add Bookmark" button to open the modal window.
3. Enter the name and URL of the website you want to bookmark.
4. Click the "Add" button to save the bookmark.
5. The bookmark will appear in the bookmarks list.
6. To delete a bookmark, click the "Delete" button next to it.
7. You can close the modal window by clicking outside of it or on the close button.

## Code Overview

The application is divided into the following parts:

- **HTML:** Contains the structure of the application, including the modal, form, and bookmarks container.
- **CSS:** Provides the styles for the application, including the layout, modal display, and bookmark items.
- **JavaScript:** Handles the functionality of the application, including adding, deleting, and fetching bookmarks, as well as form validation and event handling.

The JavaScript code is structured as follows:

- It defines variables for the modal, modal show button, modal close button, form, input fields, and bookmarks container.
- The `showModal` function is responsible for displaying the modal and focusing on the website name input field.
- Event listeners are added to the modal show button, modal close button, and window to handle the opening and closing of the modal.
- The `validate` function checks if the name and URL fields are filled and if the URL is in a valid format.
- The `buildBookmarks` function clears the bookmarks container and rebuilds it based on the current bookmarks stored in the `bookmarks` object.
- The `fetchBookmarks` function retrieves the bookmarks from the browser's local storage or creates a default bookmark if no bookmarks exist.
- The `deleteBookmark` function removes a bookmark from the `bookmarks` object and updates the local storage and bookmarks container.
- The `storeBookmark` function is triggered when the form is submitted. It retrieves the name and URL values, validates them, creates a bookmark object, adds it to the `bookmarks` object, updates the local storage and bookmarks container, and resets the form.
- An event listener is added to the form to handle the submission of a new bookmark.
- The `fetchBookmarks` function is called on page load to populate the bookmarks container with existing bookmarks.

## Conclusion

The bookmark manager provides a convenient way for users to save and organize their favorite websites. It demonstrates the use of HTML, CSS, and JavaScript to create an interactive web application with local storage functionality. Feel free to use and modify the code to suit your needs.
