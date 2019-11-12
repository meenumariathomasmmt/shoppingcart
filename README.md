import React, { Component } from 'react';
import DataTable from 'react-data-table-component';
 
const data = [{ title: 'Conan the Barbarian', year: '1982' },
{ title: 'Conan the Barbarian', year: '1981' },
{ title: 'Adfdgfg the Barbarian', year: '1982' },
{  title: 'Hsvfhd the Barbarian', year: '1820' },
{ title: 'Fasdbs the Barbarian', year: '1982' },
{ title: 'Xfsdfs the Barbarian', year: '2000' },
{ title: 'Gsudfuie the Barbarian', year: '1000' },
{ title: 'Yusducf the Barbarian', year: '2000' },
{  title: 'Absdfd the Barbarian', year: '2500' },
{ title: 'Conan the Barbarian', year: '4545' },
{  title: 'Conan the Barbarian', year: '4500' },
{  title: 'Cefer the Barbarian', year: '5660' },
{  title: 'Cfdsy the Barbarian', year: '5678' },
{  title: 'Conan the Barbarian', year: '4566' },
{  title: 'Conan sdfse Barbarian', year: '4354' },
{  title: 'Adtsdf the Barbarian', year: '7864' }];
const columns = [
  {
    name: 'Title',
    selector: 'title',
    sortable: true,
  },
  {
    name: 'Year',
    selector: 'year',
    sortable: true,
    right: true,
  },
];
const paginationOptions = { rowsPerPageText: 'Entries per page', rangeSeparatorText: 'of' };
 
class MyComponent extends Component {
  render() {
    return (
      <DataTable
        title="Entries"
        columns={columns}
        data={data}
        pagination
        paginationComponentOptions={paginationOptions}
      />
    )
  }
};
export default MyComponent;
