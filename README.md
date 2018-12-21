# psdatatranspring
## 2. Mastering Transactions
### 4 Spring Framework Advantages
Isolation levels
- DEFAULT: default from underlying database
- READ_UNCOMMITTED: Read uncommitted changes
- READ_COMMITTED: Read only committed changes
- REPEATABLE_READ: Read identical values multiple times
- SERIALIZABLE: Read identical rows multiple times

### 6 Demo: Spring Boot
```
@RestCotroller
@RequestMapping("/a")
public class Track{
  @Autowired
  
  @GetMapping("/ticket")
  public ResponseEntity<List<Ticket>> getAllTicket(){
    List<Ticket> list = ticketService.getAllTickets();
    return new ResponseEntity<List<Ticket>>(list,HttpStatus.OK)
  }
}
```
