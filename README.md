# Ceramic Tutorial Project

Welcome to the Ceramic Tutorial project! This tutorial will guide you through building a decentralized web application using Ceramic, a decentralized data network. By the end of this tutorial, you'll have a working web application that allows users to create and update their profiles on the Ceramic Network.
## Project Overview

The Ceramic Tutorial project is built using Next.js, a React framework for web applications. It guides you through creating a web application that connects users to their Ethereum wallets using Web3Modal and allows them to create and update their profiles on the Ceramic Network. Key features and components of the project include:

- **Connection to Ceramic Network**: Users can connect their Ethereum wallets to Ceramic using Web3Modal.

- **Profile Data Management**: The application uses Ceramic Streams to create and update user profiles, including profile names.

- **User-Friendly UI**: The user interface is designed for clarity and ease of use, with a navigation bar, profile display, and input fields for updating data.

## Getting Started

Follow these steps to set up and run the Ceramic Tutorial project on your local machine.

### Prerequisites

Before you begin, ensure you have the following installed:

- Node.js: [Download and install Node.js](https://nodejs.org/)

### Installation

1. Clone the repository to your local machine:

   ```bash
   git clone <repository-url>
   ```

2. Navigate to the project directory:

   ```bash
   cd ceramic-tutorial
   ```

3. Install project dependencies:

   ```bash
   npm install
   ```

4. Start the development server:

   ```bash
   npm run dev
   ```

5. Open your web browser and go to [http://localhost:3000](http://localhost:3000) to access the Ceramic Tutorial application.

## Project Structure

The project is organized as follows:

- **`pages`**: Contains Next.js pages and routes.
  - **`_app.js`**: The entry point of the application, used to wrap components with global providers.

- **`styles`**: Stores CSS styles used in the application.

- **`components`**: You can create this folder to organize React components. It contains the `RecordSetter` component.

- **`lib`**: This folder can be used to store utility functions or configuration files if needed.

## Connecting to Ceramic Network

### Web3Modal

Web3Modal simplifies the process of connecting users to their Ethereum wallets. It is initialized to connect to the Goerli Ethereum testnet, enabling users to connect to the Ceramic Network on the testnet.

### Self.ID

Self.ID is a high-level library provided by Ceramic, used to manage connections to the Ceramic Network. The `useViewerConnection` hook from Self.ID handles Ceramic connections.

### EthereumAuthProvider

The `EthereumAuthProvider` class from Self.ID connects the user's Ethereum wallet to their 3ID. It allows for signing transactions and interacting with the wallet.

## Creating and Updating Ceramic Profile Data

### RecordSetter Component

The `RecordSetter` component manages user profile data on the Ceramic Network. It uses Ceramic Streams to store and retrieve data, specifically the user's profile name. Users can input their name and click the "Update" button to update their profile.

## User Interface

The user interface (UI) is designed for user-friendliness. Key UI elements include:

- Navigation bar displaying the project title and user connection status.
- "Connect" button for connecting Ethereum wallets.
- Section displaying user information, including profile names.
- Input fields for updating profile data.
- "Update" button for updating profile data.

## Next Steps

This tutorial provides a foundation for building applications on the Ceramic Network. You can extend the project by adding more features and exploring other use cases enabled by Ceramic, such as decentralized social graphs, reputation systems, and more. Additionally, you can enhance the UI and user experience to create a polished and functional application.

Remember that Ceramic is a powerful protocol for managing decentralized data, and Self.ID simplifies the development process. You can leverage these tools to build innovative Web3 applications that offer data interoperability and security.

Enjoy exploring Ceramic and building decentralized applications!