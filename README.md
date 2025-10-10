# Simple Django Blog

Feature-rich Django blog app

## About
This repo is an adaptation of [Create A Simple Django Blog](https://www.youtube.com/playlist?list=PLCC34OHNcOtr025c1kHSPrnP18YPB-NFi) by Codemy.com

I followed the tutorial to learn followings:
- Building a feature-rich Django blog app that supports user accounts, profiles, rich posts, and social interactions — built and styled with Bootstrap.
- Implement full post CRUD (create, read, update, delete) with user authentication and permissions, threaded comments, likes/unlikes, image uploads, category pages with slugified URLs, and a polished user profile experience (profile pictures, social links and editable profile pages).
- Design as a portfolio-ready example showing how to turn tutorial scaffolding into a real, user-facing app.

### Highlights / key features

* **User accounts & authentication**
  * User registration with extended fields and Bootstrap-styled forms.
  * Login, change-password, and guarded add/edit/delete post actions so only authorized users can manage content.

* **Profiles**
  * User profile creation and edit pages with Bootstrap styling.
  * Custom profile model supporting profile pictures (default supplied) and social media links attached to posts.

* **Posts & content**
  * Add, edit, update and delete posts with title and snippet fields.
  * Rich-text editor for post bodies and HTML-aware formatting.
  * Post ordering by date and a post title/tag field for SEO/display.

* **Categories & SEO-friendly URLs**
  * Blog categories with navbar links and slugified category URLs; dedicated category pages.

* **Comments & interaction**
  * Comment section with add-comment form and related UI.
  * Like / Unlike buttons for posts (AJAX-friendly pattern implied by separate like/unlike commits).

* **Media & uploads**
  * Image upload enabled for profile pictures and post media; a default profile image shipped via static files.

* **UI & polish**
  * Bootstrap-driven styling across login, edit/add forms, and pages; various layout fixes (Firefox form-group quirks handled).
  * Navbar improvements (user’s name shown) and front-end tweaks for a cleaner UX.

### Recent development focus (map to commits)
* UI / UX polish: added user’s name to navbar, styled login and edit profile pages with Bootstrap, styled add_post form and fixed browser-specific form-group issues.
* Profile & social: created profile creation/edit pages, added default profile pic, enabled profile picture uploads, and attached social links to posts.
* Post workflow: added snippet & title fields, rich text editor, post listing and ordering, and full CRUD (add, update, delete).
* Community features: created comment form/section and like/unlike buttons.
* Content organization & routing: added categories, category pages, and slugified URLs.
* Security/permissions: added restrictions so only the correct/authenticated users can create or edit posts.
---

## How to run (dev)
1. `git clone https://github.com/webQbe/django_simpleblog.git`
2. `python -m venv .venv && source .venv/bin/activate`
3. `pip install -r requirements.txt`
4. `python manage.py migrate && python manage.py createsuperuser`
5. `python manage.py runserver`
---
Then open your browser and go to:
👉 **[http://127.0.0.1:8000/](http://127.0.0.1:8000/)**


## Credits
Original tutorial: [Create A Simple Django Blog](https://www.youtube.com/playlist?list=PLCC34OHNcOtr025c1kHSPrnP18YPB-NFi) — Codemy.com

## License
MIT License