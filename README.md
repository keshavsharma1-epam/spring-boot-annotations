# 🚀 Spring Boot Annotations Cheat Sheet (Interview Friendly)

This file contains important Spring & Spring Boot annotations explained in simple and slightly detailed words for interview preparation.

---

# 🔹 Core Spring Annotations

- `@Component` → Marks a class as a Spring bean so Spring can create and manage its object automatically.
- `@Service` → Used for business logic classes; it is a special type of `@Component`.
- `@Repository` → Used for database layer and automatically handles database exceptions.
- `@Controller` → Used in MVC applications to handle web requests and return views.
- `@RestController` → Used to build REST APIs and returns JSON instead of HTML pages.
- `@Configuration` → Marks a class that contains bean definitions for Spring.
- `@Bean` → Creates and registers a bean manually inside a configuration class.
- `@Autowired` → Automatically injects required dependency into a class.
- `@Qualifier` → Helps choose the correct bean when multiple beans of same type exist.
- `@Primary` → Makes a bean the default choice when multiple beans are available.
- `@Lazy` → Delays bean creation until it is actually needed.
- `@Scope` → Defines bean lifecycle (singleton, prototype, request, session, etc.).
- `@Value` → Injects values from application.properties file.
- `@PropertySource` → Loads external property file into Spring environment.
- `@Profile` → Loads a bean only for a specific environment (dev, test, prod).
- `@DependsOn` → Ensures one bean is created before another.
- `@Import` → Includes additional configuration classes.
- `@Order` → Defines execution priority of components.
- `@PostConstruct` → Runs a method automatically after bean initialization.
- `@PreDestroy` → Runs a method before bean is removed from memory.

---

# 🔹 Spring Boot Annotations

- `@SpringBootApplication` → Main annotation that enables auto-configuration, component scan, and configuration.
- `@EnableAutoConfiguration` → Automatically configures Spring based on dependencies present.
- `@ComponentScan` → Searches and registers components inside specified packages.
- `@ConfigurationProperties` → Maps properties from application file into Java object.
- `@EnableConfigurationProperties` → Enables use of `@ConfigurationProperties`.
- `@ConditionalOnProperty` → Loads bean only if a specific property value matches.
- `@ConditionalOnMissingBean` → Creates bean only if no other bean of same type exists.
- `@ConditionalOnClass` → Loads configuration only if a particular class is found.
- `@EnableScheduling` → Enables support for scheduled tasks.
- `@Scheduled` → Executes a method at fixed rate, delay, or cron expression.
- `@EnableAsync` → Enables asynchronous (background) execution.
- `@Async` → Runs a method in a separate thread.
- `@EnableCaching` → Turns on caching mechanism.
- `@Cacheable` → Stores method result in cache to improve performance.
- `@CachePut` → Updates cache with latest method result.
- `@CacheEvict` → Removes data from cache.

---

# 🔹 Web / REST Annotations

- `@RequestMapping` → Maps HTTP requests to controller methods.
- `@GetMapping` → Handles HTTP GET requests.
- `@PostMapping` → Handles HTTP POST requests.
- `@PutMapping` → Handles HTTP PUT requests.
- `@DeleteMapping` → Handles HTTP DELETE requests.
- `@PatchMapping` → Handles HTTP PATCH requests.
- `@RequestBody` → Converts JSON request into Java object.
- `@ResponseBody` → Converts Java object into JSON response.
- `@PathVariable` → Extracts dynamic value from URL path.
- `@RequestParam` → Extracts query parameter from request.
- `@RequestHeader` → Gets specific value from request header.
- `@ModelAttribute` → Binds form data to a model object.
- `@ResponseStatus` → Sets custom HTTP status code.
- `@CrossOrigin` → Allows API access from different domains.
- `@ExceptionHandler` → Handles specific exceptions inside controller.
- `@ControllerAdvice` → Handles exceptions globally for all controllers.
- `@RestControllerAdvice` → Global exception handler for REST APIs.
- `@InitBinder` → Customizes how request data is converted to Java objects.

---

# 🔹 JPA / Database Annotations

- `@Entity` → Marks class as database table entity.
- `@Table` → Specifies custom table name in database.
- `@Id` → Defines primary key of table.
- `@GeneratedValue` → Automatically generates primary key value.
- `@Column` → Maps class field to table column.
- `@Transient` → Prevents a field from being stored in database.
- `@OneToOne` → Defines one-to-one relationship between two entities.
- `@OneToMany` → Defines one-to-many relationship.
- `@ManyToOne` → Defines many-to-one relationship.
- `@ManyToMany` → Defines many-to-many relationship.
- `@JoinColumn` → Specifies foreign key column in relationship.
- `@JoinTable` → Specifies middle table for many-to-many mapping.
- `@Enumerated` → Stores enum as string or number in database.
- `@Lob` → Stores large objects like text or images.
- `@Embedded` → Embeds a value-type object inside entity.
- `@Embeddable` → Marks class that can be embedded.
- `@MapsId` → Maps relationship to entity’s primary key.
- `@Version` → Used for optimistic locking to prevent data conflicts.
- `@NamedQuery` → Defines static query at entity level.
- `@Query` → Defines custom JPQL or native query.
- `@Modifying` → Used for update or delete operations.
- `@EnableJpaRepositories` → Enables JPA repository support.

---

# 🔹 Validation Annotations

- `@Valid` → Triggers validation when request is received.
- `@Validated` → Enables validation at class level.
- `@NotNull` → Field must not be null.
- `@NotBlank` → Field must not be null or blank.
- `@NotEmpty` → Field must not be empty.
- `@Size` → Restricts minimum and maximum size.
- `@Min` → Sets minimum numeric value.
- `@Max` → Sets maximum numeric value.
- `@Pattern` → Validates format using regex.
- `@Email` → Ensures valid email format.
- `@Past` → Date must be in the past.
- `@Future` → Date must be in the future.

---

# 🔹 Security Annotations

- `@EnableWebSecurity` → Enables Spring Security configuration.
- `@EnableMethodSecurity` → Enables security checks at method level.
- `@PreAuthorize` → Checks user permission before method execution.
- `@PostAuthorize` → Checks permission after method execution.
- `@Secured` → Restricts access based on user roles.
- `@RolesAllowed` → Allows only specified roles to access method.

---

# 🔹 Testing Annotations

- `@SpringBootTest` → Loads full Spring Boot context for integration testing.
- `@WebMvcTest` → Tests only web layer components.
- `@DataJpaTest` → Tests only JPA repositories.
- `@MockBean` → Creates mock object inside Spring context.
- `@TestConfiguration` → Provides custom test configuration.
- `@ActiveProfiles` → Activates specific profile during testing.
- `@Transactional` → Rolls back database changes after test.
- `@Rollback` → Forces transaction rollback.
- `@BeforeEach` → Runs before every test method.
- `@AfterEach` → Runs after every test method.

---

# 📌 Purpose

Created for quick revision and strong interview preparation for Spring Boot backend roles.
