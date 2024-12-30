# GitHub Development and Collaboration Plan

This document outlines the best practices, repository structure, and collaboration guidelines for the AirHive GitHub organization.

## 1. Repository Structure
The repositories are divided by functionality to ensure clarity and maintainability.

### Main Repositories:
- **Hardware**: Contains CAD designs, mechanical schematics, PCB layouts, and assembly manuals for hardware components.
- **SoftwareDrone**: Source code for drone functionality, including autonomy, communication, and sensor integration.
- **ChargingStationSoftware**: Software for managing the drone charging station, including power management and drone docking protocols.
- **UserInterface**: Frontend application for monitoring and controlling drones and the charging station (uses web technologies like JavaScript).
- **Documentation**: Centralized repository for user manuals, guides, and technical documentation.
- **DroneStationMain**: Central repository integrating all project components and managing system-wide configurations.

### Guidelines for the Central Repository (DroneStationMain):
- **README**: Clear overview of the project, objectives, and structure.
- **Project Directory**: References to related repositories.
- **Wiki**: Centralized documentation on collaboration processes, workflows, and quick-start guides.

---

## 2. Repository Configuration
### Branching Strategy:
- `main`: Stable branch for production-ready code.
- `development`: Ongoing development and integration.
- Feature branches: Used for individual features or fixes (e.g., `feature/auto-landing`).

### Branch Protections:
- Require at least one code review before merging to `main`.
- Automated tests must pass before merging (use GitHub Actions).

### Pull Requests and Issues:
- **Pull Request Template**:
  - What does this change?
  - How was it tested?
  - Checklist for reviewers.
- **Issue Template**:
  - Description of the issue.
  - Steps to reproduce.
  - Suggested solution.
  - Priority and labels.

---

## 3. Project Management with GitHub Projects
### Using GitHub Projects:
- Create a project board for each major area:
  - Hardware Development
  - Drone Software
  - Charging Station Software
  - User Interface

### Workflow:
1. Columns: Backlog, In Progress, Review, Completed.
2. Automate movement:
   - Issues assigned move to "In Progress".
   - Closed pull requests move to "Completed".

### Labels for Issues and PRs:
- **Priority**: `High`, `Medium`, `Low`.
- **Type**: `Bug`, `Feature`, `Enhancement`, `Documentation`.
- **Area**: `Hardware`, `Software`, `Charging Station`.

---

## 4. Automation and Integrations
### GitHub Actions:
- **Continuous Integration**:
  - Run automated tests on pull requests.
  - Lint and format code automatically.
- **Continuous Deployment**:
  - Deploy stable versions of the software to testing environments.

### Integrations:
- Notifications: Integrate with Slack or Discord for issue and PR updates.
- Dependency Management: Use Dependabot to update dependencies automatically.

---

## 5. Roles and Permissions
- **Owners**: Founders with full administrative rights.
- **Collaborators**: Assigned specific permissions per repository based on role.
- Regularly review access and revoke permissions for inactive members.

---

## 6. Documentation and Onboarding
- **Centralized Documentation**: Use the Documentation repository and wiki for:
  - Project standards.
  - Coding guidelines.
  - Deployment instructions.
- **Onboarding Guide**:
  - Quick-start guide for new contributors.
  - Links to key repositories and workflows.

---

## 7. Best Practices
### Code Reviews:
- All pull requests must be reviewed by at least one other team member.
- Use clear and constructive comments during reviews.

### Meetings:
- Weekly synchronization meetings to review progress and plan next steps.
- Use GitHub Projects to track progress during discussions.

---

This plan will help maintain organization, ensure efficient collaboration, and support scalable development for the AirHive project. Updates to this document should be proposed through pull requests.
