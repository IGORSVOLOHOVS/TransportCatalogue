# TransportCatalogue

TransportCatalogue is a C++ project that provides functionality for managing and processing transportation data. It includes features for creating a transport database, processing requests, and generating map renderings.

## Getting Started

To get started with the TransportCatalogue project, follow the instructions below.

### Prerequisites

Before building and running the project, ensure you have the following software installed on your system:

- C++ compiler with C++17 support
- CMake (version 3.10 or higher)
- Protobuf library

### Building

1. Clone the repository or download the source code.

2. Create a build directory and navigate to it:

   ```shell
   mkdir build
   cd build
   ```

3. Generate the build files using CMake:

   ```shell
   cmake ..
   ```

4. Build the project:

   ```shell
   cmake --build .
   ```

### Usage

The TransportCatalogue project supports two modes of operation: `make_base` and `process_requests`. Below are examples of how to use each mode.

#### `make_base` Mode

In `make_base` mode, you can create a transport database by providing a JSON file containing transportation data. The program reads the JSON data from standard input and builds the database.

Example usage:

```shell
./transport_catalogue make_base < transport_data.json
```

Replace `transport_data.json` with the path to your own JSON file.

#### `process_requests` Mode

In `process_requests` mode, you can process requests and obtain answers based on the previously created transport database. Requests are provided in a JSON format, and the program reads the JSON data from standard input.

Example usage:

```shell
./transport_catalogue process_requests < requests.json
```

Replace `requests.json` with the path to your own JSON file containing requests.

## Project Structure

The project consists of the following main components:

- `domain`: Contains domain objects and classes.
- `geo`: Provides functionality related to geographical data.
- `graph`: Includes graph-related algorithms and data structures.
- `json`: Handles JSON parsing and building.
- `map_renderer`: Renders map data.
- `request_handler`: Processes user requests.
- `router`: Implements the transport router.
- `serialization`: Handles serialization of data.
- `svg`: Generates SVG files for map rendering.
- `transport_catalogue`: The main application, responsible for managing the transport database and processing requests.

## Dear practicum.yandex.ru team,

Thank you for the excellent C++ development course. It was engaging, informative, and provided me with valuable skills. Grateful for the opportunity to learn with you.
