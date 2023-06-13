# onlynumbers
Program that allows the entry by the keyboard if it is only numbers

Public Class FormEjemploTeclado

    Private Sub TxtEntrada_KeyPress(ByVal sender As Object, ByVal e As System.Windows.Forms.KeyPressEventArgs) Handles TxtEntrada.KeyPress

        If Not (IsNumeric(e.KeyChar)) Then
            e.Handled = True
        End If
    End Sub

End Class
