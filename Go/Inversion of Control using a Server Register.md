```go
package main

import (
	"fmt"
)

type Database interface {
	GetData() string
}

type MySQLDatabase struct{}

func (d *MySQLDatabase) GetData() string {
	return "Data from MySQL Database"
}

type PostgresDatabase struct{}

func (d *PostgresDatabase) GetData() string {
	return "Data from Postgres Database"
}

type ServiceLocator struct {
	registry map[string]Database
}

func NewServiceLocator() *ServiceLocator {
	return &ServiceLocator{
		registry: make(map[string]Database),
	}
}

func (s *ServiceLocator) Register(databaseType string, database Database) {
	s.registry[databaseType] = database
}

func (s *ServiceLocator) Get(databaseType string) Database {
	return s.registry[databaseType]
}

type Service struct {
	Locator *ServiceLocator
}

func (s *Service) Get(serviceType string) {
	return s.Locator.Get(databaseType)
}

func main() {
	serviceLocator := NewServiceLocator()

	mysqlDB := &MySQLDatabase{}
	serviceLocator.Register("mysql", mysqlDB)

	service := &Service{Locator: serviceLocator}
	service.Get("mysql")
}

```