# DemoResourceGroup
terraform {
  required_providers {
    azurerm = {
      source = "hashicorp/azurerm"
      version = "3.71.0"
    }
  }
}

provider "azurerm" {
  features{}
}

resource "azurerm_resource_group" "RG" {
  name     = "example"
  location = "West Europe"
}

