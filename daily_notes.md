# Daily log of notes and things to do

## Jan 23, 2025

- WS-6013 Greet payload
  - Questions for Dylan
    - Diesel calc:
      - What does `Strip Till` and `Other` fall under for diesel calc?
      - How do I determine the value of Ndiesel, Rdiesel, and Cdiesel (amount of diesel used in each till system)?
      - What do I do for Residual diesel?
      - We have a new NutrientProduct model which has a "product_source" which links to an existing Supply model. Are these products in some way tied to existing Zonecalc models which store a blend percentage and us_gallons_per_mt ratio, or if not should I be able to calculate these values instead?
      - There is an application area under each product. Is it assumed that each Product was applied separately? Or should I apply only a single pass to each NutrientApplication and just use the largest area?
      - Same question ^ for Pesticide applications
      - Should I ignore nutrient applications that were applied with planting seeding?
    - For CaCO3 I don't see any "PrimaryNutrients" field.
      - There is a "limestone_applied" under NutrientManagment but this is not tied to a specific application...
    - Verify I use defaults for:
      - Hebicide
      - Insecticide
    - Should the state input have some sort of validation or set of choices?

## Jan 20, 2025

- KON-23 Setup Docker environement for development
  - Investigate how to provision kona service dependancies via docker compose configuration.
  - Talk to Kelly/devops about how they are planning on provisioning resources and what the options are for deploying local environments from the same repository as where production/stagining environments will be procured?
    - Could we use Minikube/K3D (Tilt?)
  - Other things to consider in the template:
    - integration tests
    - end-to-end tests
      - (chaos tests?)
    - functional, load, security, regression?

## Dec 23, 2024

- KON-6 Utilization API
  - Complete prototype
