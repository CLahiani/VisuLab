# VisuLab

Web-based demo scenario designer: build infrastructure topologies graphically (Veeam components, hypervisors, zones, links) before preparing and provisioning the actual machines.

## Usage

Open `visulab.html` in Chrome or Edge (single file, no installation, no dependencies).

- **Library**: drag and drop Veeam components (VBR, Proxy, Repository…), hypervisors (ESXi, Hyper-V, Proxmox VE), infrastructure (VM, Kubernetes, Container, Database, immutable S3…), zones (Zone, Datacenter, Room) and shapes.
- **Links**: drag from an object's green handle to another object.
- **Properties**: name, IP, role, OS, description, colors (right panel).
- **Multi-select**: marquee drag or Shift+click, then align/distribute.
- **Scenarios**: 📁 button to pick a working folder; direct JSON save (`Ctrl+S`), history in the left column, import/export.
- **Presentation**: full-screen read-only mode (🎬), privacy mode (👁).
- **Exports**: PNG/SVG image, and 🚀 Provisioning → KVM/libvirt bash script (cloud-init) or a detailed Markdown runbook.

## Structure

- `visulab.html` — the complete application (HTML/CSS/JS, dependency-free)

Scenarios are saved as JSON files in the working folder chosen via the 📁 button — they stay local and are not versioned in this repository.
