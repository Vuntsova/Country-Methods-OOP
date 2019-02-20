# Country-Methods-OOP

##Test Cases
##Test Area Valid Values - RUN TEST
def test_area_valid_values():
    assert round(usa.area(unit='km2')) == 9833520
    assert round(usa.area()) == 9833520
    assert round(usa.area(unit='mi2')) == 3796722
    assert round(usa.area(unit='acres')) == 2428879440
    assert round(usa.area(unit='hectares')) == 983352000

    assert round(canada.area(unit='km2')) == 9984670
    assert round(canada.area()) == 9984670
    assert round(canada.area(unit='mi2')) == 3855081
    assert round(canada.area(unit='acres')) == 2466213490
    assert round(canada.area(unit='hectares')) == 998467000
##Test Population Density - RUN TEST
def test_population_density():
    assert round(usa.population_density(), 2) == 33.12
    assert round(canada.population_density(), 2) == 3.52
##Test Gdp Per Capita - RUN TEST
def test_gdp_per_capita():
    assert round(usa.gdp_per_capita()) == 62014
    assert round(canada.gdp_per_capita()) == 52231
##Test Area Invalid Unit - RUN TEST
import pytest

def test_area_invalid_unit():
    with pytest.raises(InvalidAreaUnitException):
        usa.area(unit='INVALID')
