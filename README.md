# Milestone-1
Public Class frmTempConverter
    Private Sub btnExit_Click(sender As Object, e As EventArgs) Handles btnExit.Click
        End
    End Sub

    Private Sub hsbScroller_Scroll(sender As Object, e As ScrollEventArgs) Handles hsbScroller.Scroll
        Dim temp As Integer
        Dim celsius As Single

        temp = hsbScroller.Value
        txtFahrenheit.Text = temp  ' Set the value of the fahrenheit text box to the scroll bar value

        celsius = (temp - 32 / 9 * 5)
        txtCelsius.Text = Format(celsius, "##.00") ' Set the value of the celsius text box as the answer from the eqauation above


    End Sub

    Private Sub Label1_Click(sender As Object, e As EventArgs) Handles Label1.Click

    End Sub

    Private Sub frmTempConverter_Load(sender As Object, e As EventArgs) Handles MyBase.Load

    End Sub
End Class
