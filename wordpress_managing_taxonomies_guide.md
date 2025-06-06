# Managing Game Taxonomies: Categories & Tags for Your "Games" CPT

Once you've defined Custom Taxonomies for your "Games" Custom Post Type (CPT) – such as "Genre," "Platform," or "Developer" – the next step is to populate them with terms and use them to organize your game entries. This guide covers how to add and manage these terms.

## 1. Recap: Taxonomies for Games

*   **What they are:** Custom Taxonomies are like WordPress's built-in Categories and Tags but are created specifically for your "Games" CPT. They provide a structured way to group and classify your games.
    *   **Hierarchical Taxonomies (like Categories):** Allow for parent-child relationships (e.g., "Action" as a parent Genre, with "FPS" as a child).
    *   **Non-Hierarchical Taxonomies (like Tags):** Flat structure, no parent-child relationships (e.g., "PC," "Multiplayer" as Platform or Feature terms).
*   **Importance:** They are crucial for organizing your game library, enabling users to easily browse games by specific criteria, and for creating targeted archive pages.
*   **Previous Step:** You would have already *defined* these taxonomies (e.g., "Genre," "Platform") using a plugin like "Custom Post Type UI" (CPT UI) when you set up your "Games" CPT. This guide focuses on *adding terms* (the actual genres, platforms, etc.) to these defined taxonomies.

## 2. Accessing Your Custom Taxonomies in the WordPress Admin

After defining your custom taxonomies and associating them with your "Games" CPT, you can manage their terms directly from the WordPress admin menu.

*   Look for your CPT menu item (e.g., "Games").
*   Underneath it, you should see links for each associated taxonomy. For example:
    *   **Games > Genres**
    *   **Games > Platforms**
    *   **Games > Developers**

Clicking on these links will take you to the management screen for that specific taxonomy, similar to the default "Posts > Categories" screen.

## 3. Adding Terms to Hierarchical Taxonomies (e.g., "Genre")

Hierarchical taxonomies (like "Genre") allow you to create structured classifications with parent and child terms.

*   **Interface:** On the taxonomy management screen (e.g., Games > Genres), you'll typically see:
    *   A form on the left to "Add New Genre" (or your taxonomy name).
    *   A list of existing terms on the right.
*   **Adding a New Term:**
    *   **Name:** The display name for the term that users will see (e.g., "Action Games," "Role-Playing Games," "First-Person Shooter").
    *   **Slug:** The URL-friendly version of the name, automatically generated from the name if left blank, but can be customized (e.g., `action-games`, `rpg`, `first-person-shooter`). Use lowercase letters, numbers, and hyphens.
    *   **Parent [Taxonomy Name]:** This dropdown allows you to select an existing term as the parent, creating a hierarchy.
        *   Select "None" if it's a top-level term (e.g., "Action").
        *   Select an existing term (e.g., "Action") if you're adding a sub-term (e.g., "First-Person Shooter" as a child of "Action").
    *   **Description:** Optional. Some themes might display this description on the archive pages for this term. It can be useful for providing a brief overview of the genre.
*   **Examples for "Genre":**
    *   **Action** (Parent: None)
        *   **First-Person Shooter (FPS)** (Parent: Action)
        *   **Third-Person Shooter (TPS)** (Parent: Action)
        *   **Fighting Game** (Parent: Action)
    *   **Role-Playing (RPG)** (Parent: None)
        *   **Action RPG** (Parent: Role-Playing (RPG))
        *   **Tactical RPG** (Parent: Role-Playing (RPG))
        *   **JRPG** (Parent: Role-Playing (RPG))
    *   **Strategy** (Parent: None)
        *   **Real-Time Strategy (RTS)** (Parent: Strategy)
        *   **Turn-Based Strategy (TBS)** (Parent: Strategy)
    *   **Simulation** (Parent: None)
    *   **Puzzle** (Parent: None)
    *   **Sports** (Parent: None)

Click "Add New [Taxonomy Name]" to save the term. It will appear in the list on the right.

## 4. Adding Terms to Non-Hierarchical Taxonomies (e.g., "Platform," "Developer")

Non-hierarchical taxonomies (like "Platform," "Developer," or "Game Features") function like tags. They are typically simpler to add.

*   **Interface:** The management screen (e.g., Games > Platforms) is similar, but the "Parent" option is usually absent.
*   **Adding New Terms (from the management screen):**
    *   **Name:** The display name (e.g., "PC," "PlayStation 5," "Valve," "Open World").
    *   **Slug:** URL-friendly version.
    *   **Description:** Optional.
*   **Adding Terms While Editing a Game:**
    *   More commonly, terms for non-hierarchical taxonomies are added directly on the "Add New Game" or "Edit Game" screen.
    *   In the meta box for that taxonomy (e.g., "Platforms"), you can type in new terms separated by commas, or select from a list of frequently used terms.
*   **Examples:**
    *   **Platform:** PC, PlayStation 5, Xbox Series X, Nintendo Switch, Android, iOS, macOS, Linux.
    *   **Developer:** Valve, Rockstar Games, Nintendo, Ubisoft, CD Projekt Red, FromSoftware.
    *   **Game Features** (if created as a non-hierarchical taxonomy): Open World, Multiplayer, Single Player, Co-op, Indie, Early Access, Free-to-Play, VR Support.

## 5. Using Built-in Categories and Tags (If Applicable)

When you created your "Games" CPT (e.g., with CPT UI), you might have enabled support for WordPress's built-in 'Categories' and 'Tags'.

*   **Accessing Them:**
    *   **Built-in Categories:** Usually managed via **Posts > Categories**. If you use these for your "Games" CPT, they will likely be shared with your regular blog posts.
    *   **Built-in Tags:** Usually managed via **Posts > Tags**. Similarly, these would be shared.
*   **Pros and Cons:**
    *   **Pros:**
        *   Familiar interface for WordPress users.
        *   Some themes might have more robust default styling or features for built-in taxonomies.
    *   **Cons:**
        *   **Mixing Content:** The primary drawback. Your game genres could get mixed with blog post categories, making overall site organization messy and less clear.
        *   **Less Specificity:** Built-in taxonomies are generic. Custom taxonomies allow you to create classification systems specifically tailored to games (e.g., "Platform" is clearly for games, not blog posts).
    *   **Recommendation:** For CPTs like "Games," it's generally **highly recommended to use custom taxonomies** instead of the built-in ones. This keeps your content types distinct and your organizational structure clean. If you did enable built-in ones, consider disabling them for your CPT if you create specific custom taxonomies for the same purpose.

## 6. Assigning Taxonomy Terms When Adding/Editing a Game

Once your taxonomies have terms (or even if they don't yet, as you can add them on the fly for some types), you'll assign them when creating or editing a game:

*   **Location:** On the "Add New Game" or "Edit Game" screen, look for meta boxes in the right-hand sidebar. Each of your custom taxonomies (and built-in ones, if enabled) associated with the "Games" CPT will have its own box (e.g., "Genres," "Platforms," "Developer").
*   **Assigning Terms:**
    *   **Hierarchical Taxonomies (e.g., "Genres"):**
        *   You'll typically see a list of checkboxes for existing terms. Check all that apply.
        *   There's often an "+ Add New Genre" link to quickly add a new top-level or child genre directly from this screen.
    *   **Non-Hierarchical Taxonomies (e.g., "Platforms," "Developer"):**
        *   You'll see an input field where you can type term names. As you type, suggestions for existing terms might appear.
        *   Separate multiple terms with commas.
        *   Click "Add" to assign the terms.
        *   There might also be a link to "Choose from the most used [taxonomy name]" to select from a tag cloud.

## 7. Best Practices for Organizing Games with Taxonomies

*   **Be Consistent:** Establish clear guidelines for how terms are named and applied. Ensure anyone adding games follows these guidelines.
*   **User-Centric Thinking:** Design your taxonomy structure based on how you expect users to search for and browse games on your site. What terms would they use?
*   **Avoid Over-Categorization:** While detail is good, having too many very niche categories or an excessive number of terms can make navigation overwhelming. Start with broader terms and add more specific ones only if they provide real value for filtering and browsing.
*   **Don't Create Too Many Similar Terms:** Be careful about slight variations (e.g., "Action-RPG," "Action RPG," "ARPG"). Pick one standard format and stick to it. Merge or delete redundant terms.
*   **Review Regularly:** Periodically (e.g., every few months) review your list of terms for each taxonomy.
    *   Are there terms that are rarely used? Consider removing or merging them.
    *   Are there new genres or platforms emerging that need to be added?
    *   Is the hierarchy still logical?
*   **Slugs:** Keep slugs concise, descriptive, and keyword-relevant for better SEO and cleaner URLs.
*   **Singular vs. Plural:** Generally, use plural for the taxonomy name (Genres, Platforms) and singular or common usage for terms (Action, PC, Valve).

## 8. Impact on Website Navigation and Filtering

The effort you put into creating and managing your taxonomies pays off in how users interact with your site:

*   **Archive Pages:** WordPress automatically creates archive pages for each term in your public taxonomies. For example:
    *   `yourdomain.com/genre/action/` (lists all games in the "Action" genre)
    *   `yourdomain.com/platform/pc/` (lists all games on the "PC" platform)
*   **Navigation Menus:** You can add links to these taxonomy archive pages directly into your site's navigation menus (Appearance > Menus), allowing users to quickly jump to listings for their favorite genres or platforms.
*   **Front-End Filtering:** With additional plugins (e.g., FacetWP, Search & Filter Pro) or custom theme development, you can use these taxonomies to create powerful front-end filtering tools, allowing users to combine criteria (e.g., show all "Action RPGs" available on "PC").
*   **Related Content:** You can use taxonomies to display related games at the end of a game post (e.g., "More games in the Action genre").

By thoughtfully creating and managing your game taxonomies, you significantly improve the organization, browsability, and user experience of your game download website.
