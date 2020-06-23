# MySQL FullText Search Tips

- set fulltext word length at `my.ini` configuration file 

        ft_min_word_len = 1

- Create `FULLTEXT INDEX` with columns
        
        ALTER TABLE client DROP  INDEX `fulltext_client_name_designation`;

        ALTER TABLE client ADD FULLTEXT INDEX `fulltext_client_name_designation`(`name`, `designation`);

-  Rebuilding Table index 

        OPTIMIZE TABLE client;

- Use `MATCH() ... AGAINST` in Query

        SELECT * FROM client WHERE MATCH (`name`, `designation`)
                AGAINST ('+Developer -QA' IN BOOLEAN MODE);
