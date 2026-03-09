#!/bin/bash
# Script to create a new project folder with basic structure

PROJECT_NAME=$1

if [ -z "$PROJECT_NAME" ]; then
    echo "Usage: ./new-project.sh <project-name>"
    exit 1
fi

mkdir -p "$PROJECT_NAME"/{src,docs,tests}
touch "$PROJECT_NAME"/README.md

echo "Project '$PROJECT_NAME' created successfully!"
