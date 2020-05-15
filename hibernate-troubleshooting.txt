# Error and Exception: 


### - Caused by: org.hibernate.AnnotationException: No identifier specified for entity: my.cool.models.MyEntity 

  - Missing Id of Entity. Need to annotate id field with @Id `javax.persistence.Id`
  
         @Id
         private Long id;
