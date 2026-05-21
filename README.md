# Candidate-Role Qualification Ontology

## Overview

This ontology provides a structured, logical framework for matching candidates to job roles in Computer Science based on their skills and experience. It is designed to overcome the limitations of keyword-based matching and black-box LLM systems by offering:

- Transparent, explainable reasoning
- Hierarchical skill classification
- Skill-gap detection
- Role-level classification (Junior/Mid/Senior)
- Bias reduction (excludes gender, ethnicity, age)

## Ontology Structure

### Core Classes

| Class | Description |
|-------|-------------|
| Candidate | Job applicant with skills and experience |
| TechnicalSkill | Programming languages, databases, cloud tools, etc. |
| SoftSkill | Communication, teamwork, leadership, etc. |
| Role | Job roles (e.g., DataScientist, LLMEngineer) |
| RoleLevel | Junior, Mid, Senior (based on experience) |

### Key Object Properties

| Property | Domain | Range |
|----------|--------|-------|
| hasTechnicalSkill | Candidate | TechnicalSkill |
| hasSoftSkill | Candidate | SoftSkill |
| requiresTechnicalSkill | Role | TechnicalSkill |
| requiresSoftSkill | Role | SoftSkill |
| qualifiedFor (inferred) | Candidate | Role |

### Key Data Properties

| Property | Domain | Range |
|----------|--------|-------|
| hasYearsOfExperience | Candidate | integer |
| requiresYearsOfExperience | Role | integer |

## Tools Used

| Tool | Purpose |
|------|---------|
| Protégé | Ontology editing and visualization |
| OWL | Ontology language |
| HermiT Reasoner | Logical inference and validation |
| SPARQL | Query execution |

## File Information

| File | Format | Description |
|------|--------|-------------|
| candidate_role_ontology.owl | OWL | Main ontology file |

