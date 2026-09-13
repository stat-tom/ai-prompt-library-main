(Dependencies for langchain4j and H2 database)

public class DataAssistant { ... }

Example DataAssistant implementation using OpenAI chat model (API key placeholder). The assistant exposes tools for creating rooms, bookings and displaying database contents.

Example QueryTools uses H2 in-memory DB to create ROOMS and BOOKINGS tables and insert sample rows.

DataAssistantTools wraps QueryTools and provides @Tool methods to create rooms/bookings and display database contents.

The main loop demonstrates interacting with the data assistant to create rooms/bookings and show DB contents.
