# Spring Framework Errors and Exceptions

### - Caused by: java.lang.IllegalStateException: Ambiguous mapping. Cannot map 'todoController' method com.mydomain.controllers.TodoController#view(String, Model) to {GET /todo/{id}}: There is already 'greetingController' bean method

  - Both 'todoController' and 'greetingController' controller bean contains same path mapping.  In bellow code both view method will be match for path `/todo/123`

    In 'greetingController' controller

        @GetMapping("/todo/{id}")
        public String view(@PathVariable(name="id") String id, Model model) {
          model.addAttribute("id", "<"+id+">>");
          return "todoView";
        }

    In 'todoController' 
        
        @Controller
        @RequestMapping("/todo")
        public class TodoController {
          @GetMapping("/{id}")
          public String view(@PathVariable(name="id") String id, Model model) {
            model.addAttribute("id", id+ "@");
            return "todoView";
          }
         }
