# List of Annotations
| Annotation              | Description                                                                                                       |
|-------------------------|-------------------------------------------------------------------------------------------------------------------|
| `@SpringBootApplication`| Indicates a configuration class that declares one or more `@Bean` methods and also triggers auto-configuration and component scanning. |
| `@RestController`       | Combines `@Controller` and `@ResponseBody` to simplify the creation of RESTful web services.                      |
| `@RequestMapping`       | Provides routing information and is used to map web requests to specific handler classes or methods.              |
| `@GetMapping`           | A composed annotation that acts as a shortcut for `@RequestMapping(method = RequestMethod.GET)`.                  |
| `@PostMapping`          | A composed annotation that acts as a shortcut for `@RequestMapping(method = RequestMethod.POST)`.                 |
| `@PutMapping`           | A composed annotation that acts as a shortcut for `@RequestMapping(method = RequestMethod.PUT)`.                  |
| `@DeleteMapping`        | A composed annotation that acts as a shortcut for `@RequestMapping(method = RequestMethod.DELETE)`.               |
| `@PatchMapping`         | A composed annotation that acts as a shortcut for `@RequestMapping(method = RequestMethod.PATCH)`.                |
| `@Autowired`            | Marks a constructor, field, setter method, or config method as to be autowired by Spring's dependency injection facilities. |
| `@Component`            | Indicates that an annotated class is a "component". Considered as a candidate for component scanning.             |
| `@Service`              | Indicates that an annotated class is a "Service" (e.g., a business service facade).                               |
| `@Repository`           | Indicates that an annotated class is a "Repository" (e.g., a Data Access Object or DAO).                          |
| `@Configuration`        | Indicates that a class declares one or more `@Bean` methods and may be processed by the Spring container.         |
| `@Bean`                 | Indicates that a method produces a bean to be managed by the Spring container.                                    |
| `@Value`                | Indicates a default value expression for the annotated element.                                                   |
| `@PropertySource`       | Provides a declarative mechanism for adding a `PropertySource` to Spring's Environment.                           |
| `@EnableAutoConfiguration` | Enables Spring Boot’s auto-configuration mechanism.                                                         |    

# List of Repository Methods

| Method                            | Description                                                |
|-----------------------------------|------------------------------------------------------------|
| `save`                            | Saves a given entity.                                      |
| `saveAll`                         | Saves all given entities.                                  |
| `findById`                        | Retrieves an entity by its id.                             |
| `existsById`                      | Checks whether an entity with the given id exists.         |
| `findAll`                         | Returns all instances of the type.                         |
| `findAllById`                     | Returns all instances of the type with the given IDs.      |
| `count`                           | Returns the number of entities available.                  |
| `deleteById`                      | Deletes the entity with the given id.                      |
| `delete`                          | Deletes a given entity.                                    |
| `deleteAll`                       | Deletes all entities managed by the repository.            |
| `deleteAllById`                   | Deletes all instances of the type with the given IDs.      |
| `deleteAll(Iterable<? extends T> entities)` | Deletes the given entities.                      |

# Difference between `CrudRepository` and `JpaRepository`

- `CrudRepository` is a basic repository interface that provides basic CRUD operations.
- `JpaRepository` extends `CrudRepository` and adds additional JPA-specific methods.

# Commands used for Docker
To get container up and running  
    
    docker compose up -d 

To Check running containers

    docker compose ps

To open cli in a container

    docker exec -it postgres bash