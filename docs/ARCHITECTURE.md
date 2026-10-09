# Casa Sombrero — Public Architecture Overview

## Application

Casa Sombrero is built using the Next.js App Router with React and TypeScript.

The application is divided broadly into:

- immersive desktop presentation
- mobile ordering experience
- shared menu state
- reservation experience
- reusable visual components
- static restaurant content
- public visual assets

## Desktop

Desktop presentation components are organized around a central immersive world.

Individual restaurant experiences are presented as visual features rather than conventional stacked web sections.

## Mobile

Mobile ordering is route-based and optimized independently from the desktop presentation.

The mobile interface uses focused screens for:

- order mode
- dine-in
- delivery
- menus
- carts

## State

Frontend state is used for interactive menu, reservation, and order behavior.

The production application may use browser storage for temporary frontend state.

Implementation details and storage architecture are intentionally omitted from this public repository.

## Responsive Delivery

The application uses one deployment.

The root experience selects an appropriate presentation for the visitor's viewport.

This allows one domain to support both the desktop experience and mobile ordering system.

## Deployment

The production application is designed for deployment through Vercel.

The complete deployment configuration and production repository remain private.
