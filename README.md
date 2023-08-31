# DocCheck--Document-Certification-and-Verification-System\
# DocCheck: Document Certification & Verification System

## Description

DocCheck is a project that focuses on implementing an efficient anti-forgery mechanism for academic documents using blockchain, IPFS, and hash functions. The project aims to ensure document authenticity, reduce counterfeit certificates, and streamline the verification process.

## Roles

The project involves three main roles:

- **Issuer:** Responsible for creating and issuing electronic certificates.
- **Verifier:** Authenticates certificates using the provided mechanisms.
- **Student:** Receives and accesses their academic documents securely.

## Features

- **Security:** Utilizes blockchain, IPFS, and hash functions to ensure tamper-proof document storage.
- **Efficiency:** Simplifies the verification process, eliminating manual steps for verifiers.
- **Accessibility:** Enables students to easily access their verified academic documents via IPFS.
- **Transparency:** Leverages blockchain to ensure transparency and traceability in document issuance and verification.
- **Universality:** Suitable for educational institutions, employers, and government agencies to counter fraudulent certificates.

## Architecture

### Issuer Workflow

1. Submission of raw document and user's blockchain address.
2. Generation of UUID and QR code, appending them to the document.
3. Calculation of hash of the document along with QR code.
4. Upload of the document with QR code to IPFS.
5. Storage of hash value, issuer address, user address, and IPFS link.

### Verifier Workflow

1. Input of the document with QR code, UUID, issuer address, user address, and user name.
2. Computation of hash value of the document.
3. Verification of the document using blockchain and smart contracts.
4. Return of verification result to the verifier.

## Corner Cases

The system includes an "Invalidate" option, allowing issuers to revoke certificates in the event of human errors, maintaining the integrity of the certification process.

## Technologies Used

### Design Tools

- Excalidraw
- Draw.io

### Frontend

- React.js
- CSS

### Blockchain

- Ethereum
- Solidity
- Hardhat
- MetaMask
- Ethers.js

### IPFS

- IPFS Desktop

## Getting Started

To run the DocCheck system locally:

1. Clone this repository.
2. Navigate to the frontend directory and install dependencies using `npm install`.
3. Start the React app with `npm start`.
4. Connect to the Ethereum blockchain using MetaMask.
5. Interact with the system using the provided workflows.

## License

This project is licensed under the [MIT License](LICENSE).

---

Feel free to contribute and improve this project by opening issues and pull requests.
