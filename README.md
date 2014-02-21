Next/Previous Navigation (Pagination) Plugin for Morfy CMS
==========================================================

Configuration
-------------

Place the `nextprev` folder with its contents in `plugins` folder. Then update your `config.php` file:

    <?php
        return array(
    
            ...
            ...
            ...
    
            'plugins' => array(
                'markdown',
                'sitemap',
                'nextprev' // <= Activation
            ),
            'nextprev_config' => array( // <= Configuration
                'param' => 'page', // <= Page parameter name in URL
                'limit' => 5, // <= Number of posts to display per page
                'classes' => array( // <= List of item's HTML classes
                    'page_item' => 'page',
                    'nav' => 'pager',
                    'nav_prev' => 'previous',
                    'nav_next' => 'next',
                    'nav_disabled' => 'disabled'
                ),
                'labels' => array( // <= List of item's readable text or labels
                    'nav_prev' => '&larr; Previous',
                    'nav_next' => 'Next &rarr;',
                    'not_found' => '<div class="alert alert-danger"><p>Not found.</p></div>'
                )
            )
        );

Done.
