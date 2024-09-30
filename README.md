@model IEnumerable<AdmissionCollege.Models.PayMent>

@{
    ViewBag.Title = "Index";
    Layout = null;
}



<p>
    @Html.ActionLink("Create New", "Create")
</p>
<table class="table">
    <tr>
        <th>
            @Html.DisplayNameFor(model => model.FullName)
        </th>
        <th>
            @Html.DisplayNameFor(model => model.Email)
        </th>
        <th>
            @Html.DisplayNameFor(model => model.Address)
        </th>
        <th>
            @Html.DisplayNameFor(model => model.City)
        </th>
        <th>
            @Html.DisplayNameFor(model => model.State)
        </th>
        <th>
            @Html.DisplayNameFor(model => model.ZipCode)
        </th>
        <th>
            @Html.DisplayNameFor(model => model.Cardaccepted)
        </th>
        <th>
            @Html.DisplayNameFor(model => model.Nameoncard)
        </th>
        <th>
            @Html.DisplayNameFor(model => model.CreditCardNumber)
        </th>
        <th>
            @Html.DisplayNameFor(model => model.ExpMonth)
        </th>
        <th>
            @Html.DisplayNameFor(model => model.ExpYear)
        </th>
        <th>
            @Html.DisplayNameFor(model => model.CVV)
        </th>
        <th></th>
    </tr>

@foreach (var item in Model) {
    <tr>
        <td>
            @Html.DisplayFor(modelItem => item.FullName)
        </td>
        <td>
            @Html.DisplayFor(modelItem => item.Email)
        </td>
        <td>
            @Html.DisplayFor(modelItem => item.Address)
        </td>
        <td>
            @Html.DisplayFor(modelItem => item.City)
        </td>
        <td>
            @Html.DisplayFor(modelItem => item.State)
        </td>
        <td>
            @Html.DisplayFor(modelItem => item.ZipCode)
        </td>
        <td>
            @Html.DisplayFor(modelItem => item.Cardaccepted)
        </td>
        <td>
            @Html.DisplayFor(modelItem => item.Nameoncard)
        </td>
        <td>
            @Html.DisplayFor(modelItem => item.CreditCardNumber)
        </td>
        <td>
            @Html.DisplayFor(modelItem => item.ExpMonth)
        </td>
        <td>
            @Html.DisplayFor(modelItem => item.ExpYear)
        </td>
        <td>
            @Html.DisplayFor(modelItem => item.CVV)
        </td>
        <td>
            @Html.ActionLink("Edit", "Edit", new { id=item.BillingID }) |
            @Html.ActionLink("Details", "Details", new { id=item.BillingID }) |
            @Html.ActionLink("Delete", "Delete", new { id=item.BillingID })
        </td>
    </tr>
}

</table>
