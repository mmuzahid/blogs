# Hibernate Framework Error and Exception: 


### - Caused by: org.hibernate.AnnotationException: No identifier specified for entity: my.cool.models.MyEntity 

  - Missing Id of Entity. Need to annotate id field with @Id `javax.persistence.Id`
  
         @Id
         private Long id;
         
         
### - java.lang.IllegalArgumentException: org.hibernate.loader.MultipleBagFetchException: cannot simultaneously fetch multiple bags: [com.my.app.models.Post.comments, com.my.app.models.Post.tags] 

  - Multiple @OneToMany collections try to be loaded 
  
         @OneToMany
         private List<Comment> comments;
 
         @OneToMany
         private List<Tag> tags;


         var posts = query.from(post)
            .leftJoin(post.comments, comment).fetchJoin()
            .leftJoin(post.tags, tag).fetchJoin()
            .where(predicate)
            .fetch();
