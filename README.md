# 🚀 Spring Boot Annotations Cheat Sheet (Basic → Advanced)

This repository contains 100+ most important Spring & Spring Boot annotations frequently asked in interviews.  
Each annotation is explained in one line for quick revision.

---

# 🔹 Core Spring Annotations

- `@Component` → Marks a class as a Spring-managed bean.
- `@Service` → Specialized component for service layer.
- `@Repository` → Specialized component for DAO layer with exception translation.
- `@Controller` → Marks class as Spring MVC controller.
- `@RestController` → Combines `@Controller` and `@ResponseBody`.
- `@Configuration` → Marks class as configuration source.
- `@Bean` → Declares a bean inside a configuration class.
- `@Autowired` → Automatically injects dependency.
- `@Qualifier` → Specifies which bean to inject when multiple exist.
- `@Primary` → Gives higher priority to a bean.
- `@Lazy` → Delays bean initialization until required.
- `@Scope` → Defines bean scope (singleton, prototype, etc.).
- `@Value` → Injects value from properties file.
- `@PropertySource` → Loads external properties file.
- `@Profile` → Activates bean for specific environment.
- `@DependsOn` → Specifies bean initialization order.
- `@Import` → Imports additional configuration classes.
- `@Order` → Defines execution priority.
- `@PostConstruct` → Executes method after bean initialization.
- `@PreDestroy` → Executes method before bean destruction.

---

# 🔹 Spring Boot Annotations

- `@SpringBootApplication` → Combines configuration, auto-configuration, and component scan.
- `@EnableAutoConfiguration` → Enables automatic configuration.
- `@ComponentScan` → Scans packages for Spring components.
- `@ConfigurationProperties` → Binds properties to a Java class.
- `@EnableConfigurationProperties` → Enables configuration properties binding.
- `@ConditionalOnProperty` → Loads bean based on property value.
- `@ConditionalOnMissingBean` → Loads bean only if none exists.
- `@ConditionalOnClass` → Loads bean if specific class is present.
- `@EnableScheduling` → Enables scheduling support.
- `@Scheduled` → Executes method at fixed interval.
- `@EnableAsync` → Enables asynchronous processing.
- `@Async` → Runs method asynchronously.
- `@EnableCaching` → Enables caching mechanism.
- `@Cacheable` → Caches method result.
- `@CachePut` → Updates cache without skipping method execution.
- `@CacheEvict` → Removes entry from cache.

---

# 🔹 Web / REST Annotations

- `@RequestMapping` → Maps HTTP requests to handler methods.
- `@GetMapping` → Handles HTTP GET request.
- `@PostMapping` → Handles HTTP POST request.
- `@PutMapping` → Handles HTTP PUT request.
- `@DeleteMapping` → Handles HTTP DELETE request.
- `@PatchMapping` → Handles HTTP PATCH request.
- `@RequestBody` → Binds request JSON to Java object.
- `@ResponseBody` → Converts return value to JSON/XML.
- `@PathVariable` → Extracts value from URL path.
- `@RequestParam` → Extracts query parameter.
- `@RequestHeader` → Extracts request header value.
- `@ModelAttribute` → Binds form data to object.
- `@ResponseStatus` → Sets HTTP status code.
- `@CrossOrigin` → Enables CORS.
- `@ExceptionHandler` → Handles specific exceptions.
- `@ControllerAdvice` → Global exception handling.
- `@RestControllerAdvice` → Global REST exception handler.
- `@InitBinder` → Customizes data binding.

---

# 🔹 JPA / Hibernate Annotations

- `@Entity` → Marks class as database table.
- `@Table` → Specifies table name.
- `@Id` → Marks primary key.
- `@GeneratedValue` → Auto-generates primary key.
- `@Column` → Maps field to table column.
- `@Transient` → Excludes field from persistence.
- `@OneToOne` → Defines one-to-one relationship.
- `@OneToMany` → Defines one-to-many relationship.
- `@ManyToOne` → Defines many-to-one relationship.
- `@ManyToMany` → Defines many-to-many relationship.
- `@JoinColumn` → Specifies foreign key column.
- `@JoinColumns` → Defines multiple join columns.
- `@JoinTable` → Specifies join table.
- `@Enumerated` → Stores enum as string or ordinal.
- `@Lob` → Maps large object (BLOB/CLOB).
- `@Embedded` → Embeds value type in entity.
- `@Embeddable` → Marks class as embeddable.
- `@MapsId` → Maps relationship to entity ID.
- `@Version` → Enables optimistic locking.
- `@NamedQuery` → Defines static JPQL query.
- `@Query` → Defines custom query in repository.
- `@Modifying` → Marks query as update/delete operation.
- `@EnableJpaRepositories` → Enables JPA repositories.

---

# 🔹 Validation Annotations

- `@Valid` → Triggers validation on request body.
- `@Validated` → Enables validation at class level.
- `@NotNull` → Field cannot be null.
- `@NotBlank` → Field cannot be null or empty.
- `@NotEmpty` → Field cannot be empty.
- `@Size` → Restricts size of field.
- `@Min` → Minimum numeric value.
- `@Max` → Maximum numeric value.
- `@Pattern` → Validates field using regex.
- `@Email` → Validates email format.
- `@Past` → Date must be in past.
- `@Future` → Date must be in future.

---

# 🔹 Security Annotations

- `@EnableWebSecurity` → Enables Spring Security configuration.
- `@EnableMethodSecurity` → Enables method-level security.
- `@PreAuthorize` → Checks authorization before method execution.
- `@PostAuthorize` → Checks authorization after method execution.
- `@Secured` → Restricts method access by role.
- `@RolesAllowed` → Allows access to specific roles.

---

# 🔹 Testing Annotations

- `@SpringBootTest` → Loads full application context for testing.
- `@WebMvcTest` → Tests only web layer.
- `@DataJpaTest` → Tests only JPA layer.
- `@MockBean` → Mocks Spring bean in test context.
- `@TestConfiguration` → Defines test-specific configuration.
- `@ActiveProfiles` → Activates profile during testing.
- `@Transactional` → Rolls back transaction after test.
- `@Rollback` → Forces rollback after test.
- `@BeforeEach` → Runs before each test method.
- `@AfterEach` → Runs after each test method.

---

# 📌 Purpose

This repository is created for:
- Quick interview revision
- Understanding annotation usage
- Backend developer preparation
- Spring Boot concept clarity

---

⭐ If this helps you, consider giving it a star.
