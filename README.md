# 🚀 Spring Boot Annotations Cheat Sheet (Simple Words)

This list contains important Spring & Spring Boot annotations explained in very simple words.

---

# 🔹 Core Spring Annotations

- `@Component` → Tells Spring to manage this class.
- `@Service` → Used for business logic class.
- `@Repository` → Used for database access class.
- `@Controller` → Used to handle web requests.
- `@RestController` → Used to create REST APIs (returns JSON).
- `@Configuration` → Used to define configuration class.
- `@Bean` → Creates an object that Spring will manage.
- `@Autowired` → Automatically connects one class to another.
- `@Qualifier` → Chooses which object to inject.
- `@Primary` → Makes this object default choice.
- `@Lazy` → Creates object only when needed.
- `@Scope` → Defines how many objects should be created.
- `@Value` → Gets value from properties file.
- `@PropertySource` → Loads external properties file.
- `@Profile` → Runs code only in specific environment.
- `@DependsOn` → Makes one bean load before another.
- `@Import` → Adds another configuration class.
- `@Order` → Sets priority order.
- `@PostConstruct` → Runs method after object is created.
- `@PreDestroy` → Runs method before object is destroyed.

---

# 🔹 Spring Boot Annotations

- `@SpringBootApplication` → Main starting point of Spring Boot app.
- `@EnableAutoConfiguration` → Automatically sets up configuration.
- `@ComponentScan` → Searches for components in package.
- `@ConfigurationProperties` → Maps properties to a class.
- `@EnableConfigurationProperties` → Enables property mapping.
- `@ConditionalOnProperty` → Runs bean if property matches.
- `@ConditionalOnMissingBean` → Runs bean if no similar bean exists.
- `@ConditionalOnClass` → Runs bean if class is available.
- `@EnableScheduling` → Enables scheduled tasks.
- `@Scheduled` → Runs method after fixed time.
- `@EnableAsync` → Enables background processing.
- `@Async` → Runs method in background thread.
- `@EnableCaching` → Enables caching.
- `@Cacheable` → Saves result in cache.
- `@CachePut` → Updates cache.
- `@CacheEvict` → Removes value from cache.

---

# 🔹 Web / REST Annotations

- `@RequestMapping` → Connects URL with method.
- `@GetMapping` → Handles GET request.
- `@PostMapping` → Handles POST request.
- `@PutMapping` → Handles PUT request.
- `@DeleteMapping` → Handles DELETE request.
- `@PatchMapping` → Handles PATCH request.
- `@RequestBody` → Takes JSON data from request.
- `@ResponseBody` → Sends data as JSON response.
- `@PathVariable` → Gets value from URL.
- `@RequestParam` → Gets value from query parameter.
- `@RequestHeader` → Gets value from request header.
- `@ModelAttribute` → Binds form data to object.
- `@ResponseStatus` → Sets HTTP status code.
- `@CrossOrigin` → Allows frontend from other domain.
- `@ExceptionHandler` → Handles specific error.
- `@ControllerAdvice` → Handles errors globally.
- `@RestControllerAdvice` → Global error handler for REST APIs.
- `@InitBinder` → Customizes data conversion.

---

# 🔹 JPA / Database Annotations

- `@Entity` → Makes class a database table.
- `@Table` → Sets table name.
- `@Id` → Marks primary key.
- `@GeneratedValue` → Automatically generates ID.
- `@Column` → Maps field to column.
- `@Transient` → Ignores field from database.
- `@OneToOne` → One record connected to one record.
- `@OneToMany` → One record connected to many.
- `@ManyToOne` → Many records connected to one.
- `@ManyToMany` → Many records connected to many.
- `@JoinColumn` → Defines foreign key column.
- `@JoinTable` → Defines middle table.
- `@Enumerated` → Stores enum value.
- `@Lob` → Stores large data.
- `@Embedded` → Adds object inside entity.
- `@Embeddable` → Makes class usable inside entity.
- `@MapsId` → Uses ID from another entity.
- `@Version` → Prevents data conflict.
- `@NamedQuery` → Predefined query.
- `@Query` → Custom query in repository.
- `@Modifying` → Used for update/delete query.
- `@EnableJpaRepositories` → Enables JPA repositories.

---

# 🔹 Validation Annotations

- `@Valid` → Checks validation rules.
- `@Validated` → Enables validation in class.
- `@NotNull` → Value cannot be null.
- `@NotBlank` → Cannot be empty string.
- `@NotEmpty` → Cannot be empty.
- `@Size` → Limits size.
- `@Min` → Minimum number allowed.
- `@Max` → Maximum number allowed.
- `@Pattern` → Checks format using regex.
- `@Email` → Checks valid email.
- `@Past` → Date must be before today.
- `@Future` → Date must be after today.

---

# 🔹 Security Annotations

- `@EnableWebSecurity` → Turns on security.
- `@EnableMethodSecurity` → Secures methods.
- `@PreAuthorize` → Checks permission before method runs.
- `@PostAuthorize` → Checks permission after method runs.
- `@Secured` → Allows access based on role.
- `@RolesAllowed` → Allows specific roles only.

---

# 🔹 Testing Annotations

- `@SpringBootTest` → Loads full app for testing.
- `@WebMvcTest` → Tests only controller layer.
- `@DataJpaTest` → Tests only database layer.
- `@MockBean` → Creates fake object for testing.
- `@TestConfiguration` → Test-specific configuration.
- `@ActiveProfiles` → Uses specific profile for test.
- `@Transactional` → Rolls back data after test.
- `@Rollback` → Forces rollback.
- `@BeforeEach` → Runs before every test.
- `@AfterEach` → Runs after every test.

---

# 📌 Purpose

Created for quick revision and interview preparation.
